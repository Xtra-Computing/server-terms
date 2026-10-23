# Docker 停用及 Apptainer 迁移

*发布：2026-09-22* · *类型：政策*

【Docker 停用及 Apptainer 迁移】

各位好，

为了进一步明确服务器使用责任、加强权限控制，并提升 Xtra Computing 服务器的整体安全性，我们计划于 2026 年 9 月 30 日起停用普通用户的 Docker 权限。后续将统一使用 Apptainer 作为标准容器运行环境。

目前，所有 Xtra Computing 服务器均已安装 Apptainer。大家可以从现在开始直接使用，并请在停用日期前逐步将现有的 Docker workload 迁移至 Apptainer。

Apptainer 可以直接运行绝大多数 Docker/OCI 镜像，因此大多数现有容器镜像都可以在较少修改的情况下继续使用。不过，部分 Docker 特有的使用方式，例如 Docker Compose、privileged container、Docker 网络以及基于 daemon 的服务，可能需要额外调整。

我们已经准备了适用于 Xtra Computing 服务器环境的 Apptainer 迁移指南：

[Apptainer 迁移指南](../apptainer.md)

如果对 Apptainer 不熟悉，也可以使用 coding agent 协助完成已有 Docker workload 的迁移，以及常见 Docker 命令和配置的转换。

Apptainer 官方文档：
https://apptainer.org/docs/user/main/

请大家尽量在 2026 年 9 月 30 日前完成现有 Docker workload 的迁移。

如果你的 workload 存在 Apptainer 无法合理支持、且确实必须依赖 Docker 的技术需求，请在截止日期前联系服务器管理员，并说明具体使用场景。

感谢您使用 Xtra Computing 的服务器，也感谢大家的理解与配合。
