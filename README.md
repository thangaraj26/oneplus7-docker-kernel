# OnePlus 7 (guacamoleb) LineageOS 22.2 Docker Kernel Builder

Automated GitHub Actions builder to compile the Linux 4.14 kernel for the OnePlus 7 (`guacamoleb` / GM1901) running LineageOS 22.2 with full Docker and container support (`CONFIG_PID_NS`, `CONFIG_CGROUP_DEVICE`, `CONFIG_POSIX_MQUEUE`, `CONFIG_OVERLAY_FS`, and network bridges enabled).

## How to Run:
1. Create a new repository on your GitHub account (public or private).
2. Push this folder to that repository:
   ```bash
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git branch -M main
   git push -u origin main
   ```
3. In your GitHub repository:
   - Click on the **Actions** tab.
   - Select **Build OnePlus 7 Docker Kernel** in the left sidebar.
   - Click **Run workflow** -> **Run workflow**.
4. Wait ~5 to 8 minutes for the build to finish.
5. In the completed run, scroll down to **Artifacts** and download `OnePlus7-Docker-Kernel.zip`.
6. Flash `OnePlus7-Docker-Kernel.zip` directly in **Magisk App** -> Modules -> Install from storage (or via TWRP recovery), then reboot!
