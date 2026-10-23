# Docker Deprecation and Apptainer Migration

*Sent: 2026-09-22* · *Type: policy*

*English translation of the original Chinese announcement.*

[Docker Deprecation and Apptainer Migration]

Hi everyone,

To further clarify responsibilities for server use, strengthen access controls, and improve the overall security of the Xtra Computing servers, we plan to disable Docker access for regular users starting on September 30, 2026. Apptainer will become the standard container runtime.

Apptainer is already installed on all Xtra Computing servers. You can start using it now, and please gradually migrate your existing Docker workloads to Apptainer before the cutoff date.

Apptainer can directly run the vast majority of Docker/OCI images, so most existing container images can continue to be used with few changes. However, some Docker-specific usage patterns, such as Docker Compose, privileged containers, Docker networking, and daemon-based services, may require additional adjustments.

We have prepared an Apptainer migration guide for the Xtra Computing server environment:

[Apptainer migration guide](../apptainer.md)

If you are unfamiliar with Apptainer, you can also use a coding agent to help migrate existing Docker workloads and convert common Docker commands and configurations.

Official Apptainer documentation:
https://apptainer.org/docs/user/main/

Please aim to complete the migration of your existing Docker workloads before September 30, 2026.

If your workload has a technical requirement that Apptainer cannot reasonably support and genuinely requires Docker, please contact the server administrators before the deadline and describe your specific use case.

Thank you for using the Xtra Computing servers, and for your understanding and cooperation.
