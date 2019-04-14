# Visual Studio 2019 Launch Event in Fukuoka
https://fukuten.connpass.com/event/121948/

## ハンズオン
### 事前準備
- Microsoftアカウント
  - お持ちでない方はこちらから作成してください
  - https://account.microsoft.com/account?lang=ja-JP
- [Visual Studio 2019](https://visualstudio.microsoft.com/ja/)
  - macOSの方は[Visual Studio for Mac](https://visualstudio.microsoft.com/ja/vs/mac/)を使用してください
- .NET Core 2.1以上のSDK
  - Visual Studio 2019のインストール時に[ワークロード](https://docs.microsoft.com/ja-jp/visualstudio/install/workload-component-id-vs-enterprise?vs-2019&view=vs-2019)「ASP.NETとWeb開発」および「.NET Coreクロスプラットフォームの開発」を選択することでインストール可能です。
  - または[こちら](https://dotnet.microsoft.com/download)からインストール可能です

### 手順
#### 開発編
1. [Microsoft Learn](https://docs.microsoft.com/ja-jp/learn/)にアクセスし、Microsoftアカウントでログインします。
2. [ASP.NET Core を使用して Web API を構築する](https://docs.microsoft.com/ja-jp/learn/modules/build-web-api-net-core/)のハンズオンを進める。
    - ドキュメントではブラウザ内でのコーディングですが、今回はVisual Studioを使用しましょう。
    - ユニット6「Web API のアクションをテストする」でのWebAPIのテストは[Postman](https://www.getpostman.com/)などをお使いください。

#### デプロイ編 (for Windows)
1. [Azure App Service - アプリのホスティング](https://azure.microsoft.com/ja-jp/services/app-service/)にアクセスし、Microsoftアカウントでログインします。
2. 「Web Appsを今すぐ試す」をクリックします。
3. テンプレートは「空のサイト」を選択し、「Create」をクリックします。
4. 表示されたURLにアクセスし、既定のページが表示されることを確認します。
    - ページは開いたままにしておく。
5. 「発行プロファイルのダウンロード」をクリックし、`.publishsettings`ファイルをダウンロードします。
6. Visual Studio 2019の発行機能を使用して、WebAppsにデプロイします。
    - 参考 [発行設定をインポートして Azure に発行する](https://docs.microsoft.com/ja-jp/visualstudio/deployment/tutorial-import-publish-settings-azure?view=vs-2019#import-the-publish-settings-in-visual-studio-and-deploy)
7. URLに再度アクセスし、WebAPIの結果を確認します。

#### デプロイ編 (for Mac)
1. [Azure App Service - アプリのホスティング](https://azure.microsoft.com/ja-jp/services/app-service/)にアクセスし、Microsoftアカウントでログインします。
2. 「Web Appsを今すぐ試す」をクリックします。
3. テンプレートは「空のサイト」を選択し、「Create」をクリックします。
4. 表示されたURLにアクセスし、既定のページが表示されることを確認します。
    - ページは開いたままにしておく。
5. 「Git による複製またはプッシュ」をクリックし、表示されたテキストをコピーして控えておきましょう。
6. 開発編で作成したプロジェクトフォルダをGitリポジトリとして、Gitプッシュによるデプロイを行います。
    - 参考 [ローカル Git リポジトリからデプロイする](https://docs.microsoft.com/ja-jp/azure/app-service/deploy-local-git#deploy-your-project)
    - **注意 GitのURLに含まれる `$` は `%24` に置き換えてください。（URLエンコード）**
7. URLに再度アクセスし、WebAPIの結果を確認します。

#### 参考コンテンツ
- [Visual Studio で Azure に Web アプリを発行する - Learn | Microsoft Docs](https://docs.microsoft.com/ja-jp/learn/modules/publish-azure-web-app-with-visual-studio/)

### ハンズオンが早く終わった方へ
[Microsoft Learn](https://docs.microsoft.com/ja-jp/learn/)には他にも多くのコンテンツがあるので、興味あるものにチャレンジしてみましょう♪
