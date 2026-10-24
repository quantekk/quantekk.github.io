# 站点维护约定

## 提交

- 每次改动完成并且相关构建或验证通过后，立即将该改动提交为独立、说明清楚的 commit，不要积攒多个已完成改动。
- 只提交本次已验证的相关文件和改动；不要顺手提交仓库里其他未完成或未相关的用户改动。

## 页面更新时间戳（用户明确要求）

- 每次更新页面，必须同步更新该页面显示的更新时间戳，不得沿用上次发布时间。
- 时间戳使用 `Asia/Shanghai` 时区的实际更新时间，格式为 `YYYY-MM-DD HH:mm`。
- 提交和推送前，核对待发布页面的时间戳；发布后，核对线上页面显示的时间戳。

## 数独页面

- 发布文件为 `sudoku/index.html`，源项目位于 `/Users/hubertq/code2/sudu`。
- 先更新源项目 `app/page.tsx` 中的 `LAST_UPDATED`，再构建并同步单文件页面，保留既有 Jekyll front matter。
- 同时更新小程序时，也更新源项目 `miniprogram/pages/index/index.js` 中的 `LAST_UPDATED`，并保持与网页版一致。
