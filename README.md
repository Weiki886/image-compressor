# 图片压缩工具 (Image Compressor)

一个简单易用的在线图片压缩工具，完全在浏览器中运行，无需上传至服务器。

## 特性

- 🚀 纯浏览器端压缩，保护您的隐私
- 📦 支持多种输出格式（JPEG、PNG、WebP）
- 🎚️ 可调节压缩质量（1-100）
- 📏 可设置最大宽度
- 📁 支持批量处理多张图片
- 🖼️ 直观的压缩前后预览
- 💾 一键下载所有压缩后的图片

## 启动项目

### 本地运行
1. **克隆或下载项目**
   ```
   git clone https://github.com/yourusername/image-compressor.git
   cd image-compressor
   ```

2. **使用本地服务器启动**
   - 方法一：使用 Python 内置的 HTTP 服务器
     ```
     # Python 3
     python -m http.server
     
     # Python 2
     python -m SimpleHTTPServer
     ```
     然后在浏览器中访问 `http://localhost:8000`
   
   - 方法二：使用 Node.js 的 http-server
     ```
     # 全局安装 http-server（如果尚未安装）
     npm install -g http-server
     
     # 启动服务器
     http-server
     ```
     然后在浏览器中访问 `http://localhost:8080`
   
   - 方法三：直接在浏览器中打开 `index.html` 文件
     由于该工具完全在客户端运行，您也可以直接双击 `index.html` 文件在浏览器中打开

### 部署到网站
由于该项目是纯前端应用，您可以轻松部署到任何静态网站托管服务：

1. **GitHub Pages**
   ```
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```
   然后在仓库设置中启用 GitHub Pages

2. **Netlify/Vercel**
   - 在 Netlify/Vercel 中连接您的 GitHub 仓库
   - 设置部署目录为仓库根目录
   - 点击部署

3. **其他静态托管服务**
   将项目文件上传至您选择的静态网站托管服务即可

## 使用方法

### 添加图片
1. **拖放图片**：直接将图片文件拖放到上传区域
2. **选择图片**：点击"选择图片"按钮，从文件浏览器中选择一张或多张图片
3. 支持的图片格式：JPEG、PNG、WebP等常见图片格式

### 调整压缩设置
1. **压缩质量**：
   - 使用滑块调整压缩质量（1-100）
   - 值越低，压缩率越高，但图片质量可能下降
   - 值越高，图片质量越好，但文件大小减少不明显
   - 建议值：JPEG: 70-80, PNG: 80-90, WebP: 75-85

2. **最大宽度**：
   - 设置图片压缩后的最大宽度（像素）
   - 高度会按原始宽高比例自动计算
   - 如果原图小于设定宽度，将保持原始尺寸

3. **输出格式**：
   - JPEG：适合照片等色彩丰富的图像，不支持透明背景
   - PNG：适合需要保留透明度的图像，文件稍大
   - WebP：现代格式，同时支持有损和无损压缩，兼容性较新

### 执行压缩
1. 设置好参数后，点击"压缩所有图片"按钮
2. 压缩过程在本地浏览器中进行，大图片可能需要几秒钟时间
3. 压缩完成后，可以在预览区查看压缩前后的对比和文件大小变化

### 下载压缩后的图片
1. **单独下载**：点击每张图片下方的"下载"按钮，可下载单张图片
2. **批量下载**：点击"下载所有"按钮，将所有压缩后的图片打包下载

### 批量处理技巧
1. 您可以一次性添加多张图片进行批量处理
2. 压缩设置将应用于所有选中的图片
3. 可以在压缩前移除不需要的图片
4. 压缩完成后可以查看每张图片的压缩效果和大小变化

## 技术细节

该项目使用纯原生前端技术构建：
- HTML5 用于结构
- CSS3 用于样式
- JavaScript 用于图片处理功能
- HTML5 Canvas API 用于图片压缩

## 隐私说明

本工具完全在您的浏览器中运行，所有图片处理操作均在本地完成，不会上传到任何服务器，确保您的图片信息安全。

## 许可证

本项目采用 MIT 许可证。这意味着您可以自由地使用、修改和分发此代码，无论是用于个人还是商业目的，前提是保留原始许可证和版权声明。

详细信息请参阅 [LICENSE](LICENSE) 文件。

---

# Image Compressor

A simple and easy-to-use online image compression tool that runs completely in the browser without uploading to any server.

## Features

- 🚀 Browser-based compression to protect your privacy
- 📦 Multiple output formats supported (JPEG, PNG, WebP)
- 🎚️ Adjustable compression quality (1-100)
- 📏 Configurable maximum width
- 📁 Batch processing for multiple images
- 🖼️ Intuitive before/after compression preview
- 💾 One-click download for all compressed images

## Getting Started

### Running Locally
1. **Clone or download the project**
   ```
   git clone https://github.com/yourusername/image-compressor.git
   cd image-compressor
   ```

2. **Start with a local server**
   - Option 1: Using Python's built-in HTTP server
     ```
     # Python 3
     python -m http.server
     
     # Python 2
     python -m SimpleHTTPServer
     ```
     Then visit `http://localhost:8000` in your browser
   
   - Option 2: Using Node.js http-server
     ```
     # Install http-server globally (if not already installed)
     npm install -g http-server
     
     # Start the server
     http-server
     ```
     Then visit `http://localhost:8080` in your browser
   
   - Option 3: Open `index.html` directly in your browser
     Since this tool runs entirely client-side, you can also simply double-click the `index.html` file to open it in your browser

### Deploying to a Website
Since this is a pure frontend application, you can easily deploy it to any static website hosting service:

1. **GitHub Pages**
   ```
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```
   Then enable GitHub Pages in repository settings

2. **Netlify/Vercel**
   - Connect your GitHub repository in Netlify/Vercel
   - Set the deploy directory to the repository root
   - Click deploy

3. **Other Static Hosting Services**
   Upload the project files to your chosen static website hosting service

## How to Use

### Adding Images
1. **Drag and drop**: Drag image files directly into the upload area
2. **Select images**: Click "Choose Images" button to select one or more images from file browser
3. Supported image formats: JPEG, PNG, WebP and other common image formats

### Adjusting Compression Settings
1. **Compression quality**:
   - Use the slider to adjust compression quality (1-100)
   - Lower values result in higher compression but may reduce image quality
   - Higher values maintain better quality but with less size reduction
   - Recommended values: JPEG: 70-80, PNG: 80-90, WebP: 75-85

2. **Maximum width**:
   - Set the maximum width (in pixels) for the compressed image
   - Height will be calculated automatically based on original aspect ratio
   - If original image is smaller than the set width, original size will be maintained

3. **Output format**:
   - JPEG: Best for photos and color-rich images, doesn't support transparency
   - PNG: Suitable for images requiring transparency, slightly larger file size
   - WebP: Modern format supporting both lossy and lossless compression, newer compatibility

### Executing Compression
1. After setting parameters, click the "Compress All Images" button
2. Compression process happens locally in your browser, larger images may take a few seconds
3. Once complete, you can view the before/after comparison and file size changes in the preview area

### Downloading Compressed Images
1. **Individual download**: Click the "Download" button under each image to download a single image
2. **Batch download**: Click "Download All" button to download all compressed images at once

### Batch Processing Tips
1. You can add multiple images at once for batch processing
2. Compression settings will apply to all selected images
3. You can remove unwanted images before compression
4. After compression, you can check the compression effect and size change for each image

## Technical Details

This project is built with pure native front-end technologies:
- HTML5 for structure
- CSS3 for styling
- JavaScript for image processing functionality
- HTML5 Canvas API for image compression

## Privacy Statement

This tool runs entirely in your browser. All image processing operations are performed locally, and your images are never uploaded to any server, ensuring the security of your image data.

## License

This project is licensed under the MIT License. This means you are free to use, modify, and distribute this code for personal or commercial purposes as long as you include the original license and copyright notice.

See the [LICENSE](LICENSE) file for details. 