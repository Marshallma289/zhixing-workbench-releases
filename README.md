# 知行工作台 · Windows 发布

这里仅提供知行工作台的 Windows x64 安装包和应用内更新清单。应用源码在独立的私有仓库维护。

## 下载与安装

从 [最新版本](https://github.com/Marshallma289/zhixing-workbench-releases/releases/latest) 下载 `ZhixingWorkbench_版本号_x64-setup.exe`，运行安装。首次安装需 Windows Edge WebView2；安装器会在缺失时引导安装。

如果当前安装的版本没有「设置与连接 → 应用更新」，请手动安装最新版本一次；以后可在应用内检查、下载并确认更新。更新前会自动创建工作数据备份；有运行中的 Agent 或未保存修改时，请先处理后再安装。

## 发布文件

- `.exe`：Windows 安装包。
- `.exe.sig`：更新签名，由应用使用内置公钥校验。
- `latest.json`：应用读取的版本、下载地址和签名清单。

更新签名用于校验安装包完整性与版本，不等同于 Windows 发布者证书。Windows 可能仍显示“未知发布者”；请核对下载来源。

正常工作数据保存在当前用户的 `%LOCALAPPDATA%/ZhixingWorkbench`，应用内备份不包含 API 凭据。请保留自己的工作备份。

本仓库不接收 API 密钥、工作材料或个人数据。第三方许可证随安装包提供。
