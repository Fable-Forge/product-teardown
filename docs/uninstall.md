# Uninstall product-teardown

仅删除用户明确选择的运行时目录中的 `product-teardown`：

- `~/.codex/skills/product-teardown/`
- `~/.claude/skills/product-teardown/`
- `~/.agents/skills/product-teardown/`

删除前必须解析并显示绝对路径，确认目录名恰好为 `product-teardown`，且位于对应的 `skills` 根目录内。不要递归删除未验证的变量、用户主目录或整个 skills 根目录。存在本地修改时，先让用户决定是否备份。
