### Live Presentation

![External Image](https://s3.amazonaws.com/static.slid.es/logo/v2/slides-symbol-512x512.png)



## Background

[Retail Media Network](https://www.bridgewell.com/what-is-retail-media-network/)

<small>Handling the role of SSP on the app side</small>


## Challenge

- Finding talent is challenging (~~$$$~~)
- A dual-app platform requires versatile engineers
- SDK's entry barrier for development is high


### Challenge

- Outsourcing development to an advertising company - (X)
- Finding outsourced engineers on my own - (O)


## Final Decision
> Vietnamese Outsourced Engineers



## Tools Used
> 以下皆沒有付費升級解鎖
- Claude 
- ChatGPT


## Role: Dev

- Engineer Interview
- Documentation
- ~~Hands-on~~


### Interview

<small>
你是一個資深的科技業主管，負責App team的大小事情。
如今需要面試資深工程師，主要工作職責在開發廣告相關的 SDK 該具備何種技術，條列式列出
</small>

```
以下是面試資深工程師時，針對開發廣告相關SDK應具備的技術條列：

1. **編程語言**  
   - 精通 Java 或 Kotlin（Android 開發）。
   - 熟悉 Swift 或 Objective-C（iOS 開發）。
   - 了解 JavaScript 或 TypeScript（跨平台開發）。

2. **SDK 開發經驗**  
   - 有設計和實現 SDK 的實際經驗。
   - 理解 SDK 的版本管理和兼容性問題。

3. **廣告技術知識**  
   - 熟悉 OpenRTB、VAST、VPAID 和 IAB 標準。
   - 理解廣告服務器、需求方平台（DSP）和供應方平台（SSP）的運作。

4. **網絡技術**  
   - 精通 HTTP/HTTPS 協議及 RESTful API 設計。
   - 熟悉 WebSocket 和 gRPC 的使用。

5. **數據處理**  
   - 有數據追蹤和分析的經驗，熟悉工具如 Google Analytics 或 Firebase。
   - 理解用戶行為分析和數據報告生成。

6. **安全性和隱私**  
   - 了解數據加密和保護用戶隱私的最佳實踐。
   - 熟悉 GDPR、CCPA 等隱私法規及其影響。

7. **CI/CD 流程**  
   - 有使用 Jenkins、GitHub Actions 或 GitLab CI 的經驗。
   - 理解自動化測試和持續部署的概念。

8. **測試和調試**  
   - 熟悉單元測試、集成測試和性能測試的實踐。
   - 能夠使用工具進行故障排除（如 Charles、Fiddler）。

9. **跨團隊協作**  
   - 具備良好的溝通能力，能與產品經理、設計師和其他工程師協作。
   - 有敏捷開發或 Scrum 實踐的經驗。

10. **文檔撰寫**  
    - 能夠撰寫清晰的技術文檔和使用說明。
    - 熟悉 Markdown 或其他文檔格式的撰寫。

這些技術要素將幫助候選人在廣告相關SDK的開發中有效地執行工作。
```


### Interview
> 太過籠統，但是也不知道要怎麼樣讓他吐出我想要的


### Interview - In practice
- Work Experience, Project Experience, Teamwork
- Crashlytics, FCM, APNs
- Deep Link, Universal Link
- Distribute SDK
- Automate Building, Releasing


### Documentation


### Documentation

> 豆頁疼


### Documentation
<small>
你是一個開發ios的資深工程師，請幫我優化以下語句讓他是一個好閱讀的文件
</small>

```text
1. Create CSR first. [follow] (<https://developer.apple.com/help/account/create-certificates/create-a-certificate-signing-request/>)
2. Apple Developer Program > Certificates, IDs & Profiles > Certificates
3. Create Certificates, iOS Distribution (App Store Connect and Ad Hoc), Upload a Certificate Signing Request above.
4. Create Identifiers, App IDs, type: App, fill Description, Explicit Bundle ID
5. Create Profiles, App Store Connect, select the App ID created above, select the certificate created above.
6. Download xxx.mobileprovision and xxx.cer from (3) and (5)
7. Double-click xxx.cer and import it to keychain, and export it to xxx.p12 with passphrase
8. Set following github action secrets P12_PASSWORD, P12_BASE64, PROVISIONING_PROFILE_BASE64, CERTIFICATE_KEYCHAIN_PASSWORD
```


### Documentation
```
### iOS Development: Certificate and Profile Setup Guide

1. **Create a Certificate Signing Request (CSR)**  
   Follow the instructions here: [Apple Developer Documentation](https://developer.apple.com/help/account/create-certificates/create-a-certificate-signing-request/).

2. **Navigate to Apple Developer Program**  
   Go to **Certificates, IDs & Profiles** and select **Certificates**.

3. **Create a Certificate**  
   - Choose `iOS Distribution (App Store Connect and Ad Hoc)`.
   - Upload the previously created Certificate Signing Request.

4. **Create Identifiers**  
   - Go to **App IDs**.
   - Set the type to `App`.
   - Fill in the `Description` and specify an explicit `Bundle ID`.

5. **Create Profiles**  
   - Select `App Store Connect`.
   - Choose the `App ID` created in the previous step.
   - Select the certificate created in step 3.

6. **Download Necessary Files**  
   - Download the `xxx.mobileprovision` and `xxx.cer` files from steps 3 and 5.

7. **Import and Export Certificate**  
   - Double-click `xxx.cer` to import it into Keychain.
   - Export the certificate as `xxx.p12` with a passphrase.

8. **Set GitHub Action Secrets**  
   - `P12_PASSWORD`
   - `P12_BASE64`
   - `PROVISIONING_PROFILE_BASE64`
   - `CERTIFICATE_KEYCHAIN_PASSWORD`
```


### Documentation - SDK Doc
<small>
你是一個資深的科技業rd 擅長撰寫 iOS sdk 文件 幫我將以下中文轉換成英文
</small>

```text
新增 ad refreshinterval 使用範例
新增 compatible with Objective-C
API breaking change: BannerView -> BwsBannerView, BannerViewDelegate -> BwsBannerViewDelegate
新增廣告曝光與點擊的callback function 說明
僅更新文件，無新版sdk release
```


### Documentation - SDK Doc
```text
Here's the translation:

- Added example for `ad refreshInterval` usage.
- Added compatibility with Objective-C.
- API breaking change: `BannerView` -> `BwsBannerView`, `BannerViewDelegate` -> `BwsBannerViewDelegate`.
- Added documentation for the ad exposure and click callback functions.
- Documentation update only, no new SDK release.
```



## Role: PM

Spec, Spec, Spec


## Spec Generate

<small>prompt - role</small>

```text
You are a senior technology industry PM. 

Please help me translate the following Chinese description 
into clear, concise English, and improve the logical flow. 

The description should be formatted in the style of opening a 
GitHub issue, outlining the event clearly and attaching 
corresponding Acceptance Criteria (AC). 

Your goal is to ensure the description is comprehensive and 
professional for a development team to follow.
```


## Spec Generate

<small>prompt - goal</small>

```text
Chinese Text:
目前我們尚缺少一份在 GitHub 上的 Quickstart sample code。
請你先 survey 適合當成範本的 repository，討論確認後，再開始撰寫相關的程式碼。
內容包含 iOS SDK 安裝，SDK initialization，In-app Banner，In-app Sticky Bottom-Right Ad，Webview API。

初步有看到這個 repo，不知道你對這個看法如何：https://github.com/firebase/quickstart-ios/tree/main/crashlytics
```


## Spec Generate

<small>prompt - concern</small>

```text
Key Considerations:

The issue should clearly explain the task, context, 
and expectations.

Use a formal, technical tone suitable for engineers.

Ensure the Acceptance Criteria (AC) is clear and measurable.

Include all relevant technical details, links, and potential 
repositories for the survey step.

Ensure logical flow and readability.
```


## Spec - Result

```
# Create QuickStart Sample Code for SDK Integration

## Description

We currently lack a QuickStart sample code repository on GitHub for our SDK. This issue outlines the process to create this essential resource for developers.

### Context

A well-structured QuickStart guide is crucial for developer onboarding and showcasing the primary features of our SDK. This will serve as the first point of reference for developers integrating our SDK into their projects.

### Task Overview

1. Survey and identify suitable repositories to use as templates for our QuickStart guide.
2. Discuss and confirm the chosen template with the team.
3. Develop the sample code covering key SDK functionalities.

### Required SDK Functionalities

The QuickStart sample code should demonstrate the following:

- SDK installation
- SDK initialization
- In-app Banner implementation
- In-app Sticky Bottom-Right Ad integration
- Webview API usage

### Reference

For inspiration, we can review the following repository structure:
[Firebase iOS Quickstart - Crashlytics](https://github.com/firebase/quickstart-ios/tree/main/crashlytics)

## Acceptance Criteria (AC)

1. [ ] A new GitHub repository is created for the QuickStart sample code.
2. [ ] The repository includes clear, well-commented code examples for all required SDK functionalities.
3. [ ] A comprehensive README.md file is provided, containing:
   - [ ] Step-by-step installation instructions
   - [ ] Clear explanation of each sample's purpose and functionality
   - [ ] Any necessary prerequisites or dependencies
4. [ ] The code structure follows best practices and is consistent with the chosen template repository.
5. [ ] All code samples are tested and verified to work with the latest version of our SDK.
6. [ ] The repository includes appropriate licensing information.
7. [ ] Documentation includes troubleshooting tips and links to further resources (e.g., full API documentation).

## Additional Notes

- Ensure the code is platform-agnostic or provide separate examples for major platforms (iOS, Android, Web) if necessary.
- Consider including a Changelog.md to track future updates to the QuickStart guide.
- Implement CI/CD to automatically test the sample code against new SDK releases.
```


## Spec - Refine

- 確認 spec 規格正否正確
- 是否有太過分的要求
- 明確的需求，寫出來的 spec 才會好用
- 如果是 survey 類型，且目標不明確，難以控制



## Role: QA

- Code Review
- ~~Hands-on~~


### Code Review
<small>你是一個kotlin開發大師，請幫我解釋以下程式碼的內容</small>
```kotlin
private fun loadAds(inAppApi : InAppApi) {
    val vg = findViewById<ViewGroup>(R.id.frameAdWrapper)
    val displayMetrics = resources.displayMetrics

    // This is the actual config size in the XML
    val bannerWidth = (vg.width / displayMetrics.density).roundToInt()
    val bannerHeight = (vg.height / displayMetrics.density).roundToInt()
```


#### Code Review

```
這段 Kotlin 程式碼定義了一個私有函數 `loadAds`，並傳入一個名為 `inAppApi` 的參數。以下是程式碼的逐行解析：

private fun loadAds(inAppApi : InAppApi) {
    // 找到一個 ID 為 frameAdWrapper 的 ViewGroup 元素
    val vg = findViewById<ViewGroup>(R.id.frameAdWrapper)
    
    // 獲取當前設備的顯示度量資訊
    val displayMetrics = resources.displayMetrics

    // 計算在 XML 配置中實際的寬度
    val bannerWidth = (vg.width / displayMetrics.density).roundToInt()
    
    // 計算在 XML 配置中實際的高度
    val bannerHeight = (vg.height / displayMetrics.density).roundToInt()
}

主要步驟：
1. **找到 ViewGroup 元素：**
   val vg = findViewById<ViewGroup>(R.id.frameAdWrapper)
   這行程式碼使用 `findViewById` 方法，根據 ID `R.id.frameAdWrapper` 找到對應的 ViewGroup 元素，並將其存儲在 `vg` 變數中。

2. **獲取顯示度量資訊：**
   val displayMetrics = resources.displayMetrics
   `resources.displayMetrics` 獲取當前設備的顯示度量資訊，包括密度、屏幕寬高等資訊，並將其存儲在 `displayMetrics` 變數中。

3. **計算實際配置寬度：**
   val bannerWidth = (vg.width / displayMetrics.density).roundToInt()
   將 ViewGroup 的寬度除以顯示密度，計算出在 XML 配置中的實際寬度，並使用 `roundToInt()` 方法將結果四捨五入為整數，存儲在 `bannerWidth` 變數中。

4. **計算實際配置高度：**
   val bannerHeight = (vg.height / displayMetrics.density).roundToInt()

   將 ViewGroup 的高度除以顯示密度，計算出在 XML 配置中的實際高度，並使用 `roundToInt()` 方法將結果四捨五入為整數，存儲在 `bannerHeight` 變數中。

這段程式碼的主要目的是根據當前設備的顯示密度，計算出一個 ViewGroup 在 XML 中配置的實際寬高，這在顯示廣告或其他需要根據屏幕密度調整大小的情況下非常有用。
```


#### Code Review - Value

Android & iOS 顯示單位定義上的差異  
~~iOS 不用除以 density, android 要。一定是跟它不合~~

**盡可能達到雙平台實作的細節一致性**


## Hands-on
- 從頭 Setup App 做測試
- Local build
- Local Distribute
  - iOS: CocoaPods, SPM
  - Android: AAR, Maven 



### Conclustion

- `撰寫英文 spec` & `英文溝通` 上，容易許多
- Google Translate 絕對不適合寫這種東東 (被我用來驗證語句正確性)
- Google Meet Speech-to-Text 太猛
- ~~0 * N 還是 0~~
- 有些細節，沒講到關鍵點，開出來的spec 做出來還是錯的方向
