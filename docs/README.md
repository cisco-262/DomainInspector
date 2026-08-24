<div align="center">

<img src="/docs/assets/images/app-logo.png" alt="Domain Health Inspector Logo" width="120">

# Domain Health Inspector

**See Domain, DNS, HTTPS, and Mail Health at a Glance**  
**让域名、DNS、HTTPS 和邮件安全状态一眼可见**

A focused, local-first iPhone app for inspecting domain registration, expiry, DNS records, HTTP/HTTPS reachability, TLS certificates, and mail security configuration.

一款专注且本地优先的 iPhone 域名检查工具，用于查看域名注册与到期、DNS 记录、HTTP/HTTPS 可达性、TLS 证书和邮件安全配置。

<br>

[![App Store](https://img.shields.io/badge/App_Store-Download-0D96F6?logo=apple&logoColor=white)](https://apps.apple.com/us/app/domain-health-inspector/id6792293532)
[![Website](https://img.shields.io/badge/Website-domain.opshome.run-6557D2)](https://domain.opshome.run)
[![Platform](https://img.shields.io/badge/Platform-iPhone-lightgrey?logo=apple)](https://apps.apple.com/us/app/domain-health-inspector/id6792293532)
[![Storage](https://img.shields.io/badge/Storage-Local_First-success)](https://domain.opshome.run/privacy/)
[![Price](https://img.shields.io/badge/Price-Free_%2B_IAP-blue)](https://apps.apple.com/us/app/domain-health-inspector/id6792293532)

<br>

<a href="https://apps.apple.com/us/app/domain-health-inspector/id6792293532">
  <img src="https://img.shields.io/badge/Download_on_the-App_Store-000000?logo=apple&logoColor=white&style=for-the-badge" alt="Download Domain Health Inspector on the App Store">
</a>

<br><br>

<img src="/docs/IMG_0544-portrait.png" alt="Domain Health Inspector iPhone app showing a domain health report" width="300">

<br>

[English](#english) · [简体中文](#简体中文) · [Website](https://domain.opshome.run) · [Privacy](https://domain.opshome.run/privacy/) · [Support](https://domain.opshome.run/support/) · [App Store](https://apps.apple.com/us/app/domain-health-inspector/id6792293532)

</div>

---

## English

### Overview

**Domain Health Inspector** brings common domain, DNS, HTTPS, TLS, and mail-related checks into one focused iPhone app.

It is designed for people who manage:

- Personal websites
- APIs
- Home servers
- Mail domains
- Parked domains
- Small-team internet-facing assets

Instead of relying on separate lookup websites, command-line tools, and spreadsheets, you can add a domain or URL, select how it is used, and review a structured health report.

### Key Capabilities

| Capability | Description |
| --- | --- |
| **Domain registration and expiry** | Review public RDAP registration data, registrar information when available, domain status, expiry date, and remaining days. |
| **DNS record inspection** | View common DNS records grouped by type, including A, AAAA, CNAME, NS, MX, TXT, DMARC, and other publicly available records. |
| **HTTP and HTTPS checks** | Inspect website or API reachability, HTTP status, redirects, and related response information. |
| **TLS inspection** | Check TLS handshake status, certificate validity, expiry risk, issuer, subject, and other certificate details. |
| **Custom service ports** | Inspect HTTPS and TLS services that do not run only on the default port 443. |
| **Mail security checks** | Review public MX, TXT, SPF, DKIM, and DMARC-related configuration for domains used with email. |
| **Usage profiles** | Organize checks around websites, APIs, mail domains, home services, parked domains, and other common scenarios. |
| **Focused health reports** | Classify checks as normal, needing attention, disabled, or not configured instead of reducing everything to one confusing score. |
| **JSON backup and restore** | Export complete local app data for migration and restore. |
| **PDF report export** | Create a readable domain analysis report when a document copy is needed. |

### Checks Organized Around Real Domain Usage

Different domains have different purposes. A parked domain does not need the same checks as an API, and a mail domain needs different records from a home server.

Domain Health Inspector lets you choose a usage profile so that the report can focus on checks that make sense for the selected scenario.

Typical profiles include:

- Website
- API
- Mail domain
- Home service
- Parked domain
- Other internet-facing service

This keeps reports easier to read and reduces misleading warnings for checks that are irrelevant to a domain's actual purpose.

### Domain Registration and Expiry

The registration section can help you review publicly available information such as:

- RDAP registration data
- Registrar information when available
- Registration date
- Expiry date
- Remaining days
- Domain status
- Name servers

Expiry information is presented with urgency-aware states so that domains approaching expiration can be identified quickly.

RDAP and registrar data may be unavailable or inconsistent depending on the registry and registrar response.

### DNS Record Inspection

DNS results are grouped by record type so that large configurations remain readable.

Supported and commonly displayed records can include:

- A
- AAAA
- CNAME
- NS
- MX
- TXT
- SOA
- CAA
- SPF-related TXT records
- DKIM-related records
- DMARC

The report can help identify missing, unexpected, or incomplete public DNS configuration.

Domain Health Inspector reads public DNS data. It does not request access to your DNS provider account.

### HTTP and HTTPS Analysis

For websites, APIs, home services, and other public endpoints, the app can inspect:

- HTTP or HTTPS reachability
- HTTP response status
- Redirect behavior
- Response headers
- Server information when publicly exposed
- Selected service port
- TLS handshake status

You can enter a domain, full URL, or an explicit service port.

HTTPS and TLS checks depend on the selected port and public network reachability. A service that is available only inside a LAN or VPN may not be suitable for a public-domain inspection workflow.

### TLS Certificate Inspection

TLS inspection can help review:

- Handshake success or failure
- Certificate issuer
- Certificate subject
- Validity period
- Expiration date
- Remaining days
- Subject Alternative Names
- Certificate fingerprint
- Public-key information
- Certificate-related warnings

The report is intended to make certificate expiry and configuration risks easier to identify before they affect a public service.

### Mail Security Checks

For domains used with email, the app can review public mail-related configuration such as:

- MX records
- SPF
- DKIM
- DMARC
- Supporting TXT records

Mail results depend on the records that are publicly published in DNS. A record that is not configured, uses a provider-specific selector, or is intentionally absent may require manual interpretation.

### Health Report States

Domain Health Inspector does not reduce every domain to a single generic score.

Checks are organized into practical states:

| State | Meaning |
| --- | --- |
| **Normal** | The check completed and the result appears consistent with the selected use case. |
| **Needs attention** | The result may require review, correction, or renewal planning. |
| **Disabled** | Inspection for the domain or check has been paused. |
| **Not configured** | The related record or service was not detected or is not configured. |

Reports are grouped into registration, DNS, HTTP, TLS, and mail categories.

### Typical Issues the App Can Surface

Domain Health Inspector can help identify:

- Domains approaching expiry
- Missing or unexpected DNS records
- Incorrect A, AAAA, CNAME, NS, or MX configuration
- HTTPS services that are unreachable
- Unexpected HTTP responses or redirects
- TLS handshake failures
- Certificates approaching expiry
- Mail domains without expected SPF, DKIM, or DMARC configuration
- Checks that are intentionally disabled or not configured

The app presents public inspection results. It does not automatically modify DNS, renew certificates, or change registrar settings.

### Workflow

1. **Add a domain, URL, or service port**  
   Paste the domain name, full URL, or explicit port you want to inspect.

2. **Choose a usage profile**  
   Select website, API, mail, home-service, parked-domain, or another suitable scenario.

3. **Run the inspection**  
   The app queries the public endpoints needed for the selected checks.

4. **Review the health report**  
   Read registration, DNS, HTTP, TLS, and mail findings by category.

5. **Export or back up when needed**  
   Use JSON for complete migration and restore, or export a readable PDF report.

### Backup and Export

Domain Health Inspector provides two different export formats:

#### JSON Backup

JSON backup is intended for:

- Complete local backup
- Migration to another device
- Restoring the app's domain list and related local data
- Preserving inspection settings and report information

#### PDF Report

PDF export is intended for:

- Creating a readable copy of a domain report
- Sharing findings with a colleague or service provider
- Retaining a document-style analysis record
- Reviewing results outside the app

Backup and report files are created only when you choose to export them and are handled through the iOS document-sharing interface.

### Local-First Privacy

Domain Health Inspector is designed as a local-first domain asset inspection app.

The app may store the following information locally on the device:

- Domain names and URLs
- Custom service ports
- Usage profiles
- Inspection settings
- Report findings
- Report history
- Purchase entitlement state
- Language preference
- Local backup metadata

When an inspection is run, the app connects to the public DNS, RDAP, HTTP, HTTPS, TLS, and mail-related endpoints required to create the report.

Domain Health Inspector does not require:

- Account registration for local use
- Uploading the domain portfolio to a Domain Health Inspector cloud account
- Registrar passwords
- DNS provider credentials
- Certificate private keys
- Server passwords
- Packet capture
- Browsing-history collection

Local JSON storage uses iOS file-protection policies. Exported JSON and PDF files remain under the user's control after they leave the app.

Read the complete [Privacy Policy](https://domain.opshome.run/privacy/).

### What Domain Health Inspector Is Not

Domain Health Inspector is not:

- A domain registrar
- A DNS hosting provider
- A certificate authority
- A certificate-renewal automation service
- A DNS configuration editor
- A registrar-account management client
- A packet-capture tool
- A continuous background infrastructure-monitoring platform
- A guarantee that every registry or registrar will provide complete RDAP data

The app inspects public information and presents it in a structured report. Configuration changes remain the responsibility of the domain owner and relevant service providers.

### Need Continuous Infrastructure Monitoring?

Domain Health Inspector is designed for focused domain analysis and report generation.

For continuous monitoring, alerts, uptime history, public endpoints, private Docker Probe checks, Synology NAS, Proxmox VE, Linux hosts, Docker containers, and private infrastructure assets, use **OpsHome NOC**.

[Learn about OpsHome NOC](https://app.opshome.run) · [Visit OpsHome](https://opshome.run)

### App Availability

Domain Health Inspector is available on the App Store as a free download with optional in-app purchases. It is designed for iPhone and requires iOS 17 or later.

[Download Domain Health Inspector on the App Store](https://apps.apple.com/us/app/domain-health-inspector/id6792293532)

### Support

For product support:

- Visit the [Domain Health Inspector Support page](https://domain.opshome.run/support/)
- Include the app version
- Include the iOS version
- Include the device model
- Include the affected domain
- Briefly describe the expected and actual result
- Do not send registrar passwords, DNS provider credentials, private keys, server passwords, or other secrets

Common troubleshooting notes:

- Run an incomplete inspection again after confirming internet access.
- RDAP information may vary by registry or registrar.
- HTTPS and TLS results depend on the selected port and public reachability.
- Mail-security checks depend on publicly available MX, TXT, SPF, DKIM, and DMARC records.
- Export a JSON backup or PDF report before clearing local data when a copy is needed.

---

## 简体中文

### 产品介绍

**Domain Health Inspector** 将域名注册与到期、DNS、HTTP/HTTPS、TLS 证书和邮件安全检查集中到一款专注的 iPhone 应用中。

它适合管理以下资产的用户：

- 个人网站
- API
- 家庭服务器
- 邮件域名
- 停放域名
- 小团队的公网资产

无需在多个查询网站、命令行工具和表格之间切换。添加域名或 URL、选择实际用途后，即可查看结构化健康报告。

### 核心能力

| 功能 | 说明 |
| --- | --- |
| **域名注册与到期** | 查看公开 RDAP 注册信息、可用时的注册商信息、域名状态、到期日期和剩余天数。 |
| **DNS 记录检查** | 按类型查看 A、AAAA、CNAME、NS、MX、TXT、DMARC 等公开 DNS 记录。 |
| **HTTP 和 HTTPS 检查** | 检查网站或 API 可达性、HTTP 状态、跳转和相关响应信息。 |
| **TLS 检查** | 查看 TLS 握手、证书有效期、到期风险、签发者、主题和其他证书信息。 |
| **自定义服务端口** | 检查不只运行在默认 443 端口上的 HTTPS 和 TLS 服务。 |
| **邮件安全检查** | 查看邮件域名公开的 MX、TXT、SPF、DKIM 和 DMARC 配置。 |
| **用途配置** | 根据网站、API、邮件、家庭服务、停放域名等实际用途组织检查项目。 |
| **结构化健康报告** | 将结果标记为正常、需要关注、已禁用或尚未配置，而不是简单给出一个容易误解的总分。 |
| **JSON 备份与恢复** | 导出完整本地应用数据，用于迁移和恢复。 |
| **PDF 报告导出** | 需要可读文档时生成域名分析报告。 |

### 围绕真实域名用途组织检查

不同域名有不同用途。停放域名不需要和 API 完全相同的检查，邮件域名也需要不同于家庭服务器的记录。

Domain Health Inspector 允许选择用途配置，使报告集中显示适合当前场景的检查项目。

常见用途包括：

- 网站
- API
- 邮件域名
- 家庭服务
- 停放域名
- 其他公网服务

这样可以减少与实际用途无关的误导性提醒，让报告更容易阅读。

### 域名注册与到期

注册信息部分可以帮助查看公开数据，例如：

- RDAP 注册信息
- 可用时的注册商信息
- 注册日期
- 到期日期
- 剩余天数
- 域名状态
- 名称服务器

到期信息会根据紧急程度展示不同状态，方便快速发现临近到期的域名。

RDAP 和注册商信息可能因注册局、注册商响应方式不同而缺失或不一致。

### DNS 记录检查

DNS 结果按记录类型分组，复杂配置也能保持可读。

可能显示的常见记录包括：

- A
- AAAA
- CNAME
- NS
- MX
- TXT
- SOA
- CAA
- 与 SPF 相关的 TXT 记录
- DKIM 相关记录
- DMARC

报告可以帮助发现缺失、异常或配置不完整的公开 DNS 记录。

Domain Health Inspector 读取公开 DNS 数据，不会要求登录 DNS 服务商账号。

### HTTP 和 HTTPS 分析

对于网站、API、家庭服务和其他公网端点，应用可以检查：

- HTTP 或 HTTPS 可达性
- HTTP 响应状态
- 跳转行为
- 响应头
- 公开提供时的服务器信息
- 选定的服务端口
- TLS 握手状态

可以输入域名、完整 URL 或明确的服务端口。

HTTPS 和 TLS 结果取决于所选端口和公网可达性。只能在局域网或 VPN 中访问的服务，可能不适合使用公网域名检查流程。

### TLS 证书检查

TLS 检查可以帮助查看：

- 握手成功或失败
- 证书签发者
- 证书主题
- 有效期
- 到期日期
- 剩余天数
- 主题备用名称
- 证书指纹
- 公钥信息
- 证书相关提醒

报告用于帮助用户在公网服务受到影响前，发现证书到期和配置风险。

### 邮件安全检查

对于用于邮件的域名，应用可以检查公开配置，例如：

- MX
- SPF
- DKIM
- DMARC
- 相关 TXT 记录

邮件结果取决于 DNS 中公开发布的记录。如果记录尚未配置、使用特定服务商选择器，或有意不提供，可能需要人工判断。

### 健康报告状态

Domain Health Inspector 不会把所有检查简单压缩成一个通用分数。

检查结果会按照实际状态组织：

| 状态 | 含义 |
| --- | --- |
| **正常** | 检查已完成，结果与所选用途基本一致。 |
| **需要关注** | 结果可能需要检查、修正或安排续期。 |
| **已禁用** | 当前域名或检查项目已暂停。 |
| **尚未配置** | 未检测到相关记录或服务，或者尚未进行配置。 |

报告按照注册信息、DNS、HTTP、TLS 和邮件分类展示。

### 可以发现的常见问题

Domain Health Inspector 可以帮助识别：

- 域名即将到期
- DNS 记录缺失或异常
- A、AAAA、CNAME、NS 或 MX 配置错误
- HTTPS 服务无法访问
- HTTP 响应或跳转异常
- TLS 握手失败
- 证书即将到期
- 邮件域名缺少预期的 SPF、DKIM 或 DMARC 配置
- 已主动禁用或尚未配置的检查项目

应用负责检查和展示公开结果，不会自动修改 DNS、续期证书或更改注册商设置。

### 使用流程

1. **添加域名、URL 或服务端口**  
   粘贴需要检查的域名、完整 URL 或明确端口。

2. **选择用途配置**  
   选择网站、API、邮件、家庭服务、停放域名或其他合适场景。

3. **执行检查**  
   应用查询所选项目需要使用的公开端点。

4. **查看健康报告**  
   按照注册信息、DNS、HTTP、TLS 和邮件分类查看结果。

5. **按需导出或备份**  
   使用 JSON 进行完整迁移和恢复，或者导出可读的 PDF 报告。

### 备份和导出

Domain Health Inspector 提供两种不同用途的导出格式。

#### JSON 备份

JSON 备份适合：

- 完整本地备份
- 迁移到其他设备
- 恢复域名列表和相关本地数据
- 保存检查设置和报告信息

#### PDF 报告

PDF 导出适合：

- 生成可阅读的域名报告副本
- 与同事或服务商分享检查结果
- 保存文档形式的分析记录
- 在应用之外查看结果

只有用户主动选择导出时，才会创建备份和报告文件。导出的文件通过 iOS 文档分享功能处理。

### 本地优先隐私设计

Domain Health Inspector 是一款本地优先的域名资产检查应用。

应用可能在设备本地保存：

- 域名和 URL
- 自定义服务端口
- 用途配置
- 检查设置
- 报告结果
- 报告历史
- 购买权益状态
- 语言偏好
- 本地备份元数据

执行检查时，应用会连接生成报告所需的公开 DNS、RDAP、HTTP、HTTPS、TLS 和邮件相关端点。

Domain Health Inspector 不要求：

- 为本地使用注册账号
- 将域名资产列表上传到 Domain Health Inspector 云端账号
- 注册商密码
- DNS 服务商凭据
- 证书私钥
- 服务器密码
- 网络抓包
- 收集浏览历史

本地 JSON 存储使用 iOS 文件保护策略。JSON 和 PDF 文件导出后由用户自行管理。

查看完整的[隐私政策](https://domain.opshome.run/privacy/)。

### Domain Health Inspector 不是什么

Domain Health Inspector 不是：

- 域名注册商
- DNS 托管服务商
- 证书颁发机构
- 证书自动续期服务
- DNS 配置编辑器
- 注册商账号管理客户端
- 网络抓包工具
- 后台持续运行的完整基础设施监控平台
- 对所有注册局或注册商均能提供完整 RDAP 数据的保证

应用检查公开信息并整理为结构化报告。实际配置修改仍由域名所有者和相关服务商完成。

### 需要持续基础设施监控？

Domain Health Inspector 用于专注的域名分析和报告生成。

如需持续监控、告警、可用率历史、公网端点、Docker Probe 私有检查、Synology NAS、Proxmox VE、Linux 主机、Docker 容器和私有基础设施资产，请使用 **OpsHome NOC**。

[了解 OpsHome NOC](https://app.opshome.run) · [访问 OpsHome](https://opshome.run)

### App Store

Domain Health Inspector 可在 App Store 免费下载，并提供可选的 App 内购买。应用针对 iPhone 设计，需要 iOS 17 或更高版本。

[在 App Store 下载 Domain Health Inspector](https://apps.apple.com/us/app/domain-health-inspector/id6792293532)

### 支持

需要产品支持时：

- 访问 [Domain Health Inspector 支持页面](https://domain.opshome.run/support/)
- 提供应用版本
- 提供 iOS 版本
- 提供设备型号
- 提供受影响的域名
- 简要说明预期结果和实际结果
- 请勿发送注册商密码、DNS 服务商凭据、私钥、服务器密码或其他敏感信息

常见排查说明：

- 报告不完整时，确认设备可以访问互联网，然后重新执行检查。
- RDAP 信息可能因注册局或注册商不同而存在差异。
- HTTPS 和 TLS 结果取决于所选端口和公网可达性。
- 邮件安全检查依赖公开的 MX、TXT、SPF、DKIM 和 DMARC 记录。
- 清除本地数据前，如需保留副本，请先导出 JSON 备份或 PDF 报告。

---

## Website Repository

This repository contains the static product, privacy, terms, and support website for Domain Health Inspector.

本仓库包含 Domain Health Inspector 的静态产品展示、隐私政策、用户协议和支持网站。

### Published Pages

| Path | Purpose |
| --- | --- |
| `/` | English product homepage |
| `/zh-cn/` | Simplified Chinese product homepage |
| `/privacy/` | Privacy policy |
| `/terms/` | Terms of use |
| `/support/` | Product support and troubleshooting |

### Repository Structure

```text
DomainInspector/
├── README.md
└── docs/
    ├── index.html
    ├── CNAME
    ├── IMG_0544-portrait.png
    ├── favicon.ico
    ├── og.png
    ├── site.webmanifest
    ├── sitemap.xml
    ├── styles.css
    ├── privacy/
    ├── support/
    ├── terms/
    ├── zh-cn/
    └── assets/
        └── images/
            ├── app-logo.png
            ├── apple-touch-icon.png
            ├── favicon-16.png
            ├── favicon-32.png
            ├── icon-192.png
            ├── icon-512.png
            └── og.png
```

### GitHub Pages

The website is published through GitHub Pages with the custom domain:

```text
domain.opshome.run
```

The `CNAME` file, sitemap, web manifest, product pages, and support pages are stored in the `docs` directory.

---

<div align="center">

**Focused domain checks. Local-first reports. Clear next steps.**  
**专注域名检查。本地优先报告。清晰定位问题。**

[Website](https://domain.opshome.run) · [App Store](https://apps.apple.com/us/app/domain-health-inspector/id6792293532) · [Privacy](https://domain.opshome.run/privacy/) · [Support](https://domain.opshome.run/support/)

<br>

© 2026 OpsHome™. All rights reserved.

</div>
