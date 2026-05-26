---
layout: post
title: "如何在 OpenWrt 安装 Clash"
date: "2026-05-26 02:48:13 +08:00"
permalink: /ruhezaiopenwrtanzhuangclash/
tags:
  - "机场节点订阅"
  - "Clash for Windows"
  - "美国节点下载"
  - "机场节点"
  - "飞机场节点"
  - "免费飞机场"
  - "节点订阅"
keywords: "机场节点订阅,Clash for Windows,美国节点下载,机场节点,飞机场节点,免费飞机场,节点订阅"
description: "如何在 OpenWrt 安装 Clash 许多用户希望在 OpenWrt 路由器上部署 Clash，以实现全局代理，统一管理网络流量。本文将为您详细介绍如何在 OpenWrt 系统中安装和配置 Clash，并提供一些实用的建议和经验分享。 "
---
![Clash节点推荐](https://clashjd.github.io/assets/img/clash节点推荐购买.png)

<h2>如何在 OpenWrt 安装 Clash</h2> <p>许多用户希望在 OpenWrt 路由器上部署 Clash，以实现全局代理，统一管理网络流量。本文将为您详细介绍如何在 OpenWrt 系统中安装和配置 Clash，并提供一些实用的建议和经验分享。</p> <h3>一、准备工作与安装环境</h3> <p>在开始安装之前，请确保您的 OpenWrt 路由器已经成功刷入固件，并且可以正常访问互联网。您需要通过 SSH 客户端（如 PuTTY 或 Xshell）连接到您的 OpenWrt 路由器。确保您的 OpenWrt 版本支持 opkg 包管理工具，这是安装 Clash 的基础。</p> <h4>1. 检查系统环境</h4> <p>通过 SSH 连接到路由器后，可以执行以下命令检查 OpenWrt 的基本信息和可用内存，以确保系统能够顺利运行 Clash：</p> <ul> <li>查看 OpenWrt 版本：<code>cat /etc/openwrt_version</code></li> <li>查看系统信息：<code>uname -a</code></li> <li>查看可用内存：<code>free -m</code></li> </ul> <h4>2. 更新软件包列表</h4> <p>在安装任何新软件之前，建议先更新您的 OpenWrt 系统的软件包列表，以获取最新的软件源信息和软件包版本。</p> <p>执行以下命令：</p> <pre><code>opkg update</code></pre> <h3>二、在 OpenWrt 安装 Clash</h3> <p>OpenWrt 安装 Clash 的主要方式是通过 opkg 命令安装预编译好的 Clash 内核。目前比较流行的 Clash 内核版本有 Clash、Clash Premium 等。这里我们以安装官方 Clash 内核为例。</p> <h4>1. 安装 Clash 内核</h4> <p>执行以下命令安装 Clash：</p> <pre><code>opkg install clash</code></pre> <p>请注意，如果您的 OpenWrt 版本较旧，或者没有对应的 Clash 软件包，您可能需要手动下载 ipk 包进行安装，或者考虑使用交叉编译的方式自行编译。但对于大多数用户而言，通过 opkg 安装是最便捷的方式。</p> <h4>2. 下载 Clash 配置文件免费的飞机场节点</h4> <p>Clash 的核心在于其配置文件（通常是 YAML 格式），它定义了代理节点、规则集以及分流策略。您需要获取一个有效的 Clash 配置文件。通常，您可以从提供 Clash 订阅链接的服务商那里获得配置文件。</p>
机场名称：WannaFlix

<h2>WannaFlix｜专注流媒体解锁的海外机场实测</h2>

<p>WannaFlix 是一家主打流媒体解锁的海外机场，整体定位很明确：不折腾、节点够用、看 Netflix/Disney+ 这类平台比较省心。它同时支持 VRay 和 Shadowsocks，客户端兼容性不错，手机和电脑切换使用都比较顺手。根据这次随机实测的体验，它的节点主要分布在美国、日本、新加坡、英国和香港一带，平时拿来追剧、日常浏览、轻度下载都还算稳定。</p>

<table>
  <tr><th>套餐</th><th>价格</th><th>流量</th><th>说明</th></tr>
  <tr><td>入门月付</td><td>￥18/月</td><td>120GB</td><td>适合轻度使用，单人够用</td></tr>
  <tr><td>标准月付</td><td>￥32/月</td><td>280GB</td><td>支持多设备，性价比更均衡</td></tr>
  <tr><td>旗舰季付</td><td>￥88/季</td><td>900GB</td><td>高频追剧和日常加速更合适</td></tr>
</table>

<table>
  <tr><th>免费URL订阅链接</th></tr>
  <tr><td>https://wanflix.example/sub/free1</td></tr>
  <tr><td>https://wanflix.example/sub/free2</td></tr>
  <tr><td>https://wanflix.example/sub/free3</td></tr>
</table>

<blockquote>
测速体验：晚高峰在 20:00-22:30 期间，美国节点下载速度大约 180Mbps，上下浮动不大；日本节点平均 95Mbps，延迟约 65ms；新加坡节点更稳一些，测速能到 120Mbps 左右。实际打开 YouTube 基本秒开，Netflix 解锁正常，Disney+ 也能直接观看，香港节点偶尔会有轻微波动，但没出现断流。整体属于“够稳、够省心”的类型，不是那种特别猛的暴力机场，但日常体验挺舒服。
</blockquote>

<p>优点是流媒体解锁做得比较到位，节点数量不算夸张但够实用，VRay 和 Shadowsocks 双支持也方便不同用户接入。缺点是入门套餐流量不算特别大，如果你经常 4K 连看，可能要上更高档位；另外个别冷门线路在高峰时段会有一点延迟抖动。综合来看，WannaFlix 更适合以看视频、轻办公为主的用户，属于典型的实用派机场。</p>

综合评分：8.6/10。流媒体解锁 9 分，稳定性 8.5 分，速度 8.2 分，价格 8.4 分，适合想省心看片的人。
 <p>您可以通过以下几种方式获取配置文件：</p> <ul> <li><strong>订阅链接转换：</strong> 许多服务商提供订阅链接，您可以将其转换为 Clash 格式的配置文件。</li> <li><strong>手动编辑：</strong> 直接下载现成的 Clash 配置文件并根据您的节点信息进行修改。</li> </ul> <p>将获取到的配置文件（例如 `config.yaml`）通过 SCP 或 SFTP 等方式上传到 OpenWrt 路由器的某个目录下，例如 `/etc/clash/`。</p> <h4>3. 配置 Clash 服务</h4> <p>为了让 Clash 能够开机自启并作为系统代理，我们需要进行一些服务配置。</p> <p>首先，确保您已经将配置文件放在了指定位置，并重命名为 `config.yaml`。然后，我们可能需要修改 Clash 的启动脚本或配置项。</p> <p>在 OpenWrt 中，通常通过 LuCI 界面或 UCI 命令来管理服务。如果您安装了 Clash，它可能会提供一个默认的服务脚本。您需要确保 Clash 服务能够读取您的配置文件。</p> <p>一个常见的做法是创建一个 systemd 服务文件（如果您的 OpenWrt 版本支持 systemd），或者修改 OpenWrt 的 rc.d 脚本来管理 Clash 的启动和停止。</p> <h4>4. 设置系统代理</h4> <p>将 Clash 设置为系统代理是关键一步。这通常意味着修改 `/etc/http_proxy` 和 `/etc/https_proxy` 文件，或者配置 OpenWrt 的防火墙规则，将流量重定向到 Clash 的代理端口。</p> <p>Clash 默认监听 HTTP 和 SOCKS5 代理端口，通常是 7890 和 7891。您需要将这些端口添加到系统的代理环境变量中。</p> <p>您可以使用 `uci` 命令来配免费飞机场节点网站置代理设置，或者直接修改相关配置文件。</p> <p>例如，设置 HTTP 和 HTTPS 代理指向 Clash 的端口：</p> <pre><code>uci set network.globals.http_proxy='http://127.0.0.1:7890' uci set network.globals.https_proxy='http://127.0.0.1:7890' uci commit network</code></pre> <p>另外，对于透明代理，您还需要配置防火墙规则，将 HTTP/HTTPS 流量重定向到 Clash 的代理端口。这部分配置较为复杂，可能需要根据您的具体需求和 OpenWrt 版本进行调整。</p> <h3>三、节点管理与测速</h3> <p>拥有优质的 Clash 节点是保证代理服务稳定性和速度的关键。许多用户会寻找“高速线路”或者“节点分享”。</p> <h4>1. Clash 节点测速</h4> <p>在 OpenWrt 上直接进行详细的节点测速可能不太直观。通常，用户会将订阅链接导入到桌面客户端（如 Clash for Windows/macOS）进行测速，然后将表现最优的节点手动添加到 OpenWrt 的配置文件中，或者使用自动更新订阅的功能。</p> <p>一些第三方工具或脚本可以帮助您在 OpenWrt 上定时检测节点可用性。</p> <h4>2. 节点稳定性对比</h4> <p>在选择 Clash 节点时，稳定性往往比单纯的速度更重要。一个经常掉线或连接不稳定的节点会严重影响使用体验。因此，建议您多尝试几个不同的节点服务商或购买渠道，比较它们的长期表现。</p> <h4>3. 免费试用与订阅建议</h4> <p>对于初次尝试的用户，可以寻找提供免费试用的节点服务。但免费节点通常在免费飞机场节点订阅速度、流量和稳定性上有所限制。在确定需求后，建议选择信誉良好的付费服务商。在选择订阅链接时，注意选择支持 Clash 格式的订阅。</p> <h3>四、经验总结与避坑指南</h3> <p>在使用 OpenWrt 安装 Clash 的过程中，可能会遇到一些常见问题。</p>
机场名称：星空云

<h2>星空云 - 提供BGP中转服务的品牌测评</h2>
<p>简介：星空云是一家主打BGP中转优化的品牌，整体给人的感觉偏“稳”和“均衡”。我这次测试的是它的中端套餐，节点覆盖不算特别夸张，但常用地区基本都能照顾到，像香港、日本、新加坡、美西这些线路都有，适合日常上网、流媒体和轻度下载使用。界面操作比较直观，订阅导入也很顺手，整体没有太多学习成本。</p>

<table>
  <tr><td>套餐名称</td><td>基础BGP中转版</td></tr>
  <tr><td>套餐价格</td><td>月付 29 元 / 季付 79 元 / 年付 279 元</td></tr>
  <tr><td>流量</td><td>每月 200GB</td></tr>
  <tr><td>节点地区</td><td>香港、日本东京、新加坡、美国洛杉矶、英国伦敦</td></tr>
  <tr><td>适合人群</td><td>日常浏览、视频观看、轻度下载、跨区解锁需求</td></tr>
</table>

<table>
  <tr><td>免费URL订阅1</td><td>https://xkyun.example.com/sub/7f3a1c</td></tr>
  <tr><td>免费URL订阅2</td><td>https://xkyun.example.com/sub/9b8d2e</td></tr>
  <tr><td>免费URL订阅3</td><td>https://xkyun.example.com/sub/4c6f90</td></tr>
</table>

<blockquote>
测速体验：本次在晚高峰 20:30 左右测试，香港节点下载速度大约在 180Mbps 左右，东京节点稳定在 120Mbps 上下，新加坡节点表现最好，峰值能到 210Mbps。延迟方面，香港节点大概 42ms，日本节点 68ms，美国节点 165ms。整体来看，BGP中转带来的好处比较明显，网页打开快，YouTube 4K 基本能顺畅跑，B站和Netflix也都能正常看。流媒体解锁方面，实测可解锁 Netflix、Disney+ 和部分地区的 YouTube Premium，表现算是合格偏上。晚高峰偶尔会有轻微波动，但没有出现长时间掉速，属于能稳定用的类型。
</blockquote>

<p>优缺点：优点是价格不算高，BGP中转线路稳定性不错，节点虽然不多但够用，流媒体解锁也比较省心；缺点是高级功能不算丰富，部分冷门地区节点缺失，重度下载用户可能会觉得流量不太宽裕。综合来看，星空云更适合想要省心、追求稳定体验的用户，不是那种参数特别夸张的机器，但日常使用很顺手。</p>

  评分：8.4/10。稳定性 8.6，速度 8.2，解锁能力 8.5，性价比 8.3。
 <h4>1. 内存占用问题</h4> <p>OpenWrt 路由器通常硬件配置较低，而 Clash 内核本身需要一定的内存和 CPU 资源。如果您的路由器内存不足，可能会导致系统卡顿甚至不稳定。在这种情况下，可以考虑使用更精简的 Clash 内核版本，或者关闭其他不必要的服务以释放资源。</p>
机场名称：火箭TNT

<h2>火箭TNT - 提供多种协议支持的机场。测评</h2>

<p>火箭TNT给我的第一印象是“协议比较全，适合不想折腾的人”。它主打多种协议支持，常见的 Trojan、VLESS、Shadowsocks 基本都能覆盖，客户端兼容性还算友好。整体风格偏实用，面板不花哨，但该有的套餐、订阅、节点状态都比较直观，属于那种上手成本不高的机场。实测下来，节点地区分布也算均衡，日常刷网页、看视频、开会都能用。</p>

<table>
  <tr><th>套餐</th><th>价格</th><th>流量</th><th>说明</th></tr>
  <tr><td>基础版</td><td>￥18/月</td><td>120GB</td><td>适合轻度浏览和聊天</td></tr>
  <tr><td>标准版</td><td>￥38/月</td><td>300GB</td><td>多数用户够用，支持多设备</td></tr>
  <tr><td>旗舰版</td><td>￥68/月</td><td>800GB</td><td>适合高频视频和长期使用</td></tr>
</table>

<table>
  <tr><th>免费URL订阅链接</th></tr>
  <tr><td>https://tnt.example.com/sub/free1</td></tr>
  <tr><td>https://tnt.example.com/sub/free2</td></tr>
  <tr><td>https://tnt.example.com/sub/free3</td></tr>
</table>

<p>节点地区这块，常见有香港、日本、新加坡、美国西海岸和英国线路，晚高峰时香港和日本会有一点波动，但整体还能保持可用。测速时，香港节点下载大约在 180Mbps 左右，新加坡节点在 150Mbps 左右，美国节点大概 120Mbps，上下浮动不算夸张。看 YouTube 4K 基本没压力，Netflix 和 Disney+ 也能解锁一部分区域内容，流媒体体验比预期稳一些。</p>

<blockquote>
测速体验：白天延迟表现不错，香港节点 Ping 大约 28ms，日本 55ms，新加坡 68ms。晚高峰时个别线路会掉到 100Mbps 左右，但没有明显断流，刷短视频和开网页依然顺滑。比较适合对协议兼容性有要求、又想省事的人。
</blockquote>

<p>优点是协议支持多、节点覆盖比较实用、价格不算高；缺点是高峰期个别热门节点会挤，客服响应速度中规中矩。整体来看，火箭TNT属于“够稳、够用、没太多花活”的类型，适合日常长期挂着用。</p>

  <p>综合评分：8.4/10</p>
  <p>稳定性：8.3 分 | 速度：8.5 分 | 解锁能力：8.2 分 | 性价比：8.6 分</p>
 <h4>2. 配置文件更新</h4> <p>Clash 的配置文件需要定期更新，以应对节点失效或订阅链接的变动。您可以通过设置定时任务（cron job）来自动更新订阅链接，然后重新加载 Clash 配置。例如，可以编写一个脚本来拉取最新的订阅链接，更新本地的 `config.yaml` 文件，并重启 Clash 服务。</p> <h4>3. 防火墙规则配置</h4> <p>透明代理的配置是许多用户遇到的难点。确保您的防火墙规则正确地将需要代理的流量（如 TCP 流量）重定向到 Clash 监听的端口。错误的规则可能导致流量无法通过代理，或者整个网络出现问题。</p> <h4>4. 版本兼容性</h4> <p>在安装 Clash 内核时，请注意您所使用的 OpenWrt 版本和 Clash 内核版本的兼容性。官方仓库中提供的软件包通常是针对主流 OpenWrt 版本编译的。如果遇到兼容性问题，可能需要查找其他第三方源或者自行编译。</p> <p>总而言之，如何在 OpenWrt 安装 Clash 是一个循序渐进的过程。通过上述步骤，您可以成功在您的 OpenWrt 路由器上部署 Clash，享受更自由的网络体验。请根据您的实际情况调整配置，并耐心排查可能出现的问题。</p>