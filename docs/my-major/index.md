# 专业介绍

我们邀请了优秀学长以视频和文字的形式为大家分享他们的经验和见解，学长们将结合自己的学习经历，详细介绍自动化专业的独特特点、课程设置以及未来的就业方向和发展前景。

## 学长讲专业



<div style="text-align: center;">
    <div style="font-size: 1em; font-weight: bold;">2020级本科生 朱少廷（现在清华大学攻读博士）</div>
    <video style="width: 80%; height: auto; display: block; margin: auto;" controls loop>
        <source src="video/2023zst.mp4" type="video/mp4">
        您的浏览器不支持该视频播放，请升级您的浏览器。
    </video>
    <br>
    <div style="font-size: 1em; font-weight: bold;">2019级本科生、2023级研究生 周靳</div>
    <video style="width: 80%; height: auto; display: block; margin: auto;" controls loop>
        <source src="video/2023zj.mp4" type="video/mp4">
        您的浏览器不支持该视频播放，请升级您的浏览器。
    </video>
    <br>
    <div style="font-size: 1em; font-weight: bold;">2018级本科生、2022级研究生 忻铄</div>
    <video style="width: 80%; height: auto; display: block; margin: auto;" controls loop>
        <source src="video/2023xs.mp4" type="video/mp4">
        您的浏览器不支持该视频播放，请升级您的浏览器。
    </video>
</div>

## 学长眼中的“自动化”
<!-- <div class="image-gallery">
    <img src="img/2024czt.jpg" alt="Image 1">
    <img src="img/2024wpc.jpg" alt="Image 2">
    <img src="img/2024jzm.jpg" alt="Image 3">
    <img src="img/2024xtq.jpg" alt="Image 4">
    <img src="img/2024wzh.jpg" alt="Image 5">
    <img src="img/2024wrk.jpg" alt="Image 6">
    <img src="img/2024ybh.jpg" alt="Image 7">
    <img src="img/2023sjy.png" alt="Image 8">
    <img src="img/2023fgf.png" alt="Image 9">
    <img src="img/2023txs.png" alt="Image 10">
    <img src="img/2023xsj.png" alt="Image 11">
    <img src="img/2023zyj.png" alt="Image 12">
</div>

<style>
    .image-gallery {
        display: flex;
        flex-direction: column; 
        align-items: center;
        margin: 20px;
    }

    .image-gallery img {
        max-width: 80%; 
        margin: 10px 0; 
        border-radius: 8px;
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
    }
</style> -->

<div class="carousel">
    <div class="carousel-images" id="carouselImages">
        <img src="img/2024czt.jpg" alt="Image 1">
        <img src="img/2024wpc.jpg" alt="Image 2">
        <img src="img/2024jzm.jpg" alt="Image 3">
        <img src="img/2024xtq.jpg" alt="Image 4">
        <img src="img/2024wzh.jpg" alt="Image 5">
        <img src="img/2024wrk.jpg" alt="Image 6">
        <img src="img/2024ybh.jpg" alt="Image 7">
        <img src="img/2023sjy.png" alt="Image 8">
        <img src="img/2023fgf.png" alt="Image 9">
        <img src="img/2023txs.png" alt="Image 10">
        <img src="img/2023xsj.png" alt="Image 11">
        <img src="img/2023zyj.png" alt="Image 12">
    </div>
    <div class="carousel-buttons">
        <button class="button" onclick="prevSlide()">❮</button>
        <button class="button" onclick="nextSlide()">❯</button>
    </div>
</div>

## 培养方案
<iframe src="pdf/2024auto.pdf#navpanes=0" 
        width="100%" height="600px" 
        style="border: none; overflow: auto;">
    您的浏览器不支持 PDF 查看，请下载 PDF 文件: 
    <a href="pdf/2024auto.pdf">下载 PDF</a>
</iframe>

<p>
    <strong>如需离线查看或保存该文件，请点击以下链接：</strong>
    <a href="pdf/2024auto.pdf">下载 PDF 文件</a>
</p>

## 思维导图

为了帮助学生更好地理解课程结构和培养目标，学院绘制了思维导图以直观地展示了各个核心课程之间的关系。如有任何疑问，欢迎随时联系学长学姐或加入我们的QQ咨询群，获取更多信息和建议！

<img src="img/2024mindmap.jpg" alt="思维导图" style="width: 80%; display: block; margin: auto;">






<script>
    let currentIndex = 0;

    const images = document.querySelectorAll('#carouselImages img');
    const totalSlides = images.length;

    // 动态设置每张图片的宽度
    const setImageWidth = () => {
        const carouselImages = document.getElementById('carouselImages');
        const widthPercentage = 100 / totalSlides; // 计算每张图片的宽度百分比
        images.forEach(img => {
            img.style.width = `${widthPercentage}%`;
        });
        carouselImages.style.width = `${totalSlides * 100}%`; // 设置整体宽度
    };

    const showSlide = index => {
        const slides = document.querySelector('.carousel-images');

        if (index >= totalSlides) {
            currentIndex = 0;
        } else if (index < 0) {
            currentIndex = totalSlides - 1;
        } else {
            currentIndex = index;
        }

        slides.style.transform = `translateX(-${currentIndex * (100 / totalSlides)}%)`;
    };

    const nextSlide = () => {
        showSlide(currentIndex + 1);
    };

    const prevSlide = () => {
        showSlide(currentIndex - 1);
    };

    // 每3秒切换一次图片
    setInterval(nextSlide, 3000); 
    setImageWidth(); // 初始化设置图片宽度
</script>