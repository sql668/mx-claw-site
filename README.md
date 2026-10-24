# mx-claw 产品官网

静态产品官网，介绍 mx-claw 的定位、功能、工作方式、安全边界和常见问题。

本地预览：

```bash
python3 -m http.server 4173
```

打开 `http://127.0.0.1:4173`。

官网源码保留在主仓库的 `website/` 目录，公开部署仓库为
[`sql668/mx-claw-site`](https://github.com/sql668/mx-claw-site)。该公开仓库只包含静态官网
文件，并使用自己的 GitHub Actions 工作流发布 GitHub Pages。

正式地址：

```text
https://sql668.github.io/mx-claw-site/
```

修改内容时保持以下约束：

- 不依赖后端接口或第三方脚本。
- 所有站内资源使用相对路径，确保 GitHub Pages 子路径部署可用。
- 不宣称完全离线；模型请求仍会发送到用户配置的 Provider。
- 不把当前专有许可证描述成开源许可证。
- 键盘导航、移动端布局和 `prefers-reduced-motion` 必须保持可用。
