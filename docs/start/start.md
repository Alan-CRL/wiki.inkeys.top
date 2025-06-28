# 5 分钟内快速上手 :partying_face:

准备好，我们开始了~ :alarm_clock:

---

## 第一步：下载 智绘教Inkeys

智绘教Inkeys 支持 Windows 7 RTM(sp0) 及以上版本。

### 准备

在下方的网页中，选择合适的 __系统架构__ 版本，并下载。  
提供 `64位` `32位` `Arm64` 版本，需要下载匹配的版本。  

<div class="grid cards" markdown>

-   :material-download:{ .lg .middle } __123云盘下载（推荐）__

    ---

    链接为免登录不限速设计，点击下载即可

    [:octicons-arrow-right-24: 前往下载](https://www.123pan.com/s/duk9-n4dAd.html){ target="_blank" }

-   :material-book-edit:{ .lg .middle } Github Release

    [查看 Github Release](https://github.com/Alan-CRL/Inkeys/releases){ target="_blank" }

</div>

{==

<div id="arch-hint"></div>

<script>

function isWindows() 
{
    // 多数浏览器现代userAgent都同时含有Windows
    let ua = navigator.userAgent.toLowerCase();
    let platform = (navigator.platform||"").toLowerCase();
    return ua.indexOf('windows') !== -1 || platform.indexOf('win') !== -1;
}
function detectArch() 
{
    let ua = navigator.userAgent;
    let platform = navigator.platform||"";
    if (/x86_64|Win64|WOW64|amd64|x64/i.test(ua+platform)) 
    {
        return "x86_64";
    }
    if (/arm64|aarch64/i.test(ua+platform)) 
    {
        return "arm64";
    }
    if (/i686|i386|x86/i.test(ua+platform)) 
    {
        return "x86";
    }
    return "unknown";
}

var msg = "";
if (!isWindows()) 
{
    msg = "Windows 下可以帮你自动识别系统架构（当前访问设备为非 Windows，智绘教Inkeys 适用于 Windows）";
} 
else 
{
    var arch = detectArch();
    if(arch=='x86') {
        msg = "<b>检测到您的系统架构为 32位</b>，请下载 <b>32位</b> 安装包。";
    }
    else if(arch=='x86_64') {
        msg = "<b>检测到您的系统架构为 64位</b>，请下载 <b>64位</b> 安装包。";
    }
    else if(arch=='arm64') {
        msg = "<b>检测到您的系统架构为 Arm64</b>，请下载 <b>Arm64</b> 安装包。";
    }
    else {
        msg = "未能识别您的架构，通常来说很多人电脑的架构都是 64位，请尝试下载 <b>64位</b> 安装包。";
    }
}
document.getElementById('arch-hint').innerHTML = msg;

</script>

==}

??? note "我该如何手动确定系统的架构？"
    - [百度一下](https://www.baidu.com/s?wd=%E5%A6%82%E4%BD%95%E6%9F%A5%E7%9C%8B%20Windows%20%E6%9E%B6%E6%9E%84){ target="_blank" }
    - 自己搜搜：__如何查看 Windows 架构__

### 下载

1. 选择合适的版本并选择下载  
![123云盘](start/1.png){ width="48%" } ![Github Release](start/2.png){ width="48%" }  

2. 下载完成后会得到一个压缩包。![](start/3.png){ width="50%" align=right }   

### 解压

1. 使用解压软件，将软件解压出来。![](start/4.png){ width="50%" align=right }  
2. 打开解压后的文件夹，即可看到运行文件。![](start/5.png){ width="50%" align=right }  

---

??? note "`Tips.txt` 文件中包含使用提示和 CI/CD 详细信息"
    CI/CD（自动构建） 包含构建的软件版本，构建时间和构建系统等等。![](start/6.png){ width="30%" align=right }

## 启动 智绘教Inkeys

双击 `Inkeys.exe` 即可启动程序。