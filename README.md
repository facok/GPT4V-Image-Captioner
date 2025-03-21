# GPT4V-Image-Captioner / GPT4V图像打标器

A simple tool utilizing the GPT-4-vision API to generate captions for images.
This project is built with Gradio, and parts of the code were generated by GPT.

Developers: Jiaye and [LEOSAM是只兔狲](https://civitai.com/user/LEOSAM). Welcome everyone to add more new features to this project.

这是一款利用 GPT-4-vision API 为图像打标的简易工具。
使用 Gradio 构建，部分代码由 GPT 辅助生成。

![1 (2)](https://github.com/jiayev/GPT4V-Image-Captioner/assets/16369810/fa98e5db-8247-4f20-a9f5-b056c31209d6)

# Installation and Startup Guide

### Windows (If the automatic installation fails, please refer to the [Manual Installation Instructions](#windows-manual-installation-instructions))

1. Open Command Prompt as administrator and navigate to the directory where you want to clone the repository.
2. Clone the repository using the following command:
    ```
    git clone https://github.com/jiayev/GPT4V-Image-Captioner
    ```
3. Double-click `install_windows.bat` to run and install all necessary dependencies.
4. After the installation is complete, you can launch the GPT4V-Image-Captioner by double-clicking `install_windows.bat`.
5. Hold down Ctrl and click on the URL in the terminal (or copy the URL to your browser), which will open the Gradio app interface in your default browser.
6. Enter the official OpenAI or third-party GPT-4V API Key and API Url at the top of the interface. After setting the image address, you can start tagging the image.

### Linux / macOS

1. Open a terminal and navigate to the directory where you want to clone the repository.
2. Clone the repository using the following command:
    ```
    git clone https://github.com/jiayev/GPT4V-Image-Captioner
    ```
3. Navigate to the cloned directory:
    ```
    cd GPT4V-Image-Captioner
    ```
4. Make the install and start scripts executable with the following command:
    ```
    chmod +x install_linux_mac.sh; chmod +x start_linux_mac.sh
    ```
5. Execute the install script:
    ```
    ./install_linux_mac.sh
    ```
6. Launch the GPT4V-Image-Captioner in the terminal by executing the launch script:
    ```
    ./start_linux_mac.sh
    ```
7. Copy the URL displayed in the terminal and open it in your browser to access the Gradio app interface.
8. Enter the official OpenAI or third-party GPT-4V API Key and API Url at the top of the interface. After setting the image address, you can start tagging the image.

# 安装和启动指南

### Windows（如自动安装失败，请参考[手动安装说明](#windows-手动安装说明)）

1. 以管理员权限打开命令提示符，并导航到您想要克隆仓库的目录。
2. 使用以下命令克隆仓库：
    ```
    git clone https://github.com/jiayev/GPT4V-Image-Captioner
    ```
3. 双击 `install_windows.bat` 运行，并安装所有必要的依赖项。
4. 安装完成后，您可以通过双击 `Start_windows.bat`来在终端中启动GPT4V-Image-Captioner。
5. 按住ctrl并点击终端中的URL地址（或复制URL地址在浏览器打开），将在默认浏览器中跳转打开Gradio应用界面。
6. 请在界面最上方输入OpenAI官方或者第三方的GPT-4V API Key与API Url，设置图像地址后，就可以图像打标了。

### Linux / macOS

1. 打开终端，并导航到您想要克隆仓库的目录。
2. 使用以下命令克隆仓库：
    ```
    git clone https://github.com/jiayev/GPT4V-Image-Captioner
    ```
3. 导航到克隆的目录：
    ```
    cd GPT4V-Image-Captioner
    ```
4. 使用以下命令使安装脚本和启动脚本变为可执行：
    ```
    chmod +x install_linux_mac.sh; chmod +x Start_linux_mac.sh
    ```
5. 执行安装脚本：
    ```
    ./install_linux_mac.sh
    ```
6. 在终端中执行启动脚本来启动GPT4V-Image-Captioner。
    ```
    ./Start_linux_mac.sh
    ```
7. 复制终端中显示的URL地址，在浏览器中打开Gradio应用界面。
8. 请在界面最上方输入OpenAI官方或者第三方的GPT-4V API Key与API Url，设置图像地址后，就可以图像打标了。

## Change Log

### January 2, 2024
- **One-Click Install & Launch**: Added one-click installation (`install_windows.bat` / `install_linux_mac.sh`) and launch (`Start_windows.bat` / `Start_linux_mac.sh`) features, simplifying the setup and startup process.
- **Environment Setup Instructions**: Supplemented the installation and launch instructions for the program under Windows and Linux environments.

### January 1, 2024
- **Speed Optimization**: Improved the speed of tagging images. Now annotations can be completed within 2-3 seconds.
- **Tag Management**: Provided different handling options for images with existing tags: "Overwrite", "Prepend", "Append", and "Skip".
- **Subfolder Processing**: The new program can now process all image files within folders and subfolders, supporting formats like '.png', '.jpg', '.jpeg', '.webp', '.bmp', '.gif', '.tiff', '.tif'.
- **Interruption Feature**: Added the ability to interrupt the batch tagging process.
- **Error Screening**: Images that fail GPT tagging (e.g., NSFW content) can be moved to a new folder based on keywords.
- **Localization**: Added support for the Chinese language.

## 更新内容

### 2024年1月2日
- **一键安装和一键启动**: 增加了一键安装 (`install_windows.bat` / `install_linux_mac.sh`) 和一键启动 (`Start_windows.bat` / `Start_linux_mac.sh`) 功能，简化了程序的安装和启动过程。
- **环境说明补充**: 补充了在Windows和Linux环境下程序的安装和启动说明。

### 2024年1月1日
- **运行加速**: 提高了程序的打标速度。现在可以在2-3秒内完成一张图片的标注。
- **标签处理**: 对于已有标签的图像文件，提供了以下不同处理选项："覆盖", "前置插入", "结尾追加" 和 "跳过"。
- **子文件夹处理**: 新程序能够处理文件夹及其子文件夹中的所有图像文件，支持的图像格式包括：'.png', '.jpg', '.jpeg', '.webp', '.bmp', '.gif', '.tiff', '.tif'。
- **程序中断**: 增加了在批量打标签过程中中断打标的功能。
- **报错筛查**: 可以根据关键词，将所有GPT标记失败的图像（例如NSFW内容）移动到新的文件夹中。
- **本地化**: 增加了对中文的支持。


### Windows Manual Installation Instructions

1. Open the Command Prompt by pressing `Win + R`, typing `cmd`, and then pressing `Enter`.

2. Clone the repository to your local machine using the following command:
    ```
    git clone https://github.com/jiayev/GPT4V-Image-Captioner
    ```

3. Once cloning is complete, navigate to the cloned directory:
    ```
    cd GPT4V-Image-Captioner
    ```

4. Before installing any dependencies, make sure that Python is installed on your system. Check for Python's presence by typing the following command and pressing `Enter` in the Command Prompt:
    ```
    python --version
    ```
   If Python is not installed, you will get an error message. In that case, please visit the [Python official download page](https://www.python.org/downloads/) and follow the instructions to install it.

5. Create a virtual environment named `myenv` to avoid contaminating the global Python environment:
    ```
    python -m venv myenv
    ```

6. Activate the virtual environment you just created:
    ```
    myenv\Scripts\activate
    ```

7. Update `pip` to date:
    ```
    python -m pip install --upgrade pip
    ```

8. Install the `requests`, `gradio`, and `tqdm` libraries within the virtual environment:
    ```
    pip install scipy networkx wordcloud matplotlib Pillow tqdm gradio requests
    ```

9. After completing the steps above, you can start GPT4V-Image-Captioner by double-clicking the `Start_windows.bat` file.



### Windows 手动安装说明

1. 按 `Win + R` 打开命令提示符。键入 `cmd` 然后按 `Enter` 。

2. 使用下面的命令克隆仓库至本地：
    ```
    git clone https://github.com/jiayev/GPT4V-Image-Captioner
    ```

3. 克隆完成后，切换到克隆的目录中：
    ```
    cd GPT4V-Image-Captioner
    ```

4. 在安装依赖库之前，在命令提示符中输入以下命令并按 `Enter` 来检查是否电脑已经安装了 Python：
    ```
    python --version
    ```
   如果未安装，会显示错误信息。请访问 [Python 官方下载页面](https://www.python.org/downloads/) 并按照指示进行安装。

5. 创建一个名为 `myenv` 的虚拟环境以避免污染全局 Python 环境：
    ```
    python -m venv myenv
    ```

6. 激活你刚创建的虚拟环境：
    ```
    myenv\Scripts\activate
    ```

7. 更新 `pip`至最新版本：
    ```
    python -m pip install --upgrade pip
    ```

8. 在虚拟环境中安装 `requests`、`gradio` 、 `tqdm` 等库：
    ```
    pip install scipy networkx wordcloud matplotlib Pillow tqdm gradio requests
    ```

9. 完成上述步骤后，可通过双击 `Start_windows.bat` 文件来启动 GPT4V-Image-Captioner。
