# リリースベースのワークフローを作成する

_GitLabフローを基礎として構築されたリリースベースのワークフローを作成します。_

## ようこそ

GitLabフローを基盤として、リリースベースのワークフローを作成しましょう。
チームでリリースベースのワークフローを使用すると、GitHub はプロジェクトのデプロイ可能なイテレーションを容易に共同作業できる環境を提供します。
これらのイテレーションをパッケージ化し、より幅広いユーザーがダウンロードして使用できるようにすることができます。

GitHub リリースを使用すると、チームはプロジェクトの履歴の特定の時点に基づいてソフトウェアをパッケージ化し、ユーザーに提供できます。

- 対象者：開発者、DevOps エンジニア、IT 運用担当者、マネージャー、およびチーム。
- 学習内容：リリースベースのワークフローの進め方。
- 構築内容：タグ、リリース、リリースノートを作成します。
- 前提条件：ブランチ、コミット、プルリクエストについて学習する必要がある場合は、まず「GitHub 入門」を受講してください。
- 所要時間：このコースは 1 時間以内で完了します。

このコースでは、次のことを行います。

1. ベータ版リリースを作成する
2. リリースに機能を追加する
3. リリース プルリクエストを開く
4. リリースノートを追加してmainブランチにマージする
5. 検証環境ブランチにマージする
6. ホットフィックスをコミットする
7. ホットフィックスリリースをコミットする
8. ホットフィックスリリースを検証環境ブランチにマージする
9. 商用環境ブランチにマージする

## このコースのはじめかた

<!-- For start course, run in JavaScript:
'https://github.com/new?' + new URLSearchParams({
  template_owner: 'kuboctopus',
  template_name: 'release-based-gitlab-workflow',
  owner: '@me',
  name: 'skills-release-based-gitlab-workflow',
  description: 'My clone repository',
  visibility: 'public',
}).toString()
-->

[![start-course](https://user-images.githubusercontent.com/1221423/235727646-4a590299-ffe5-480d-8cd5-8194ea184546.svg)](https://github.com/new?template_owner=kuboctopus&template_name=release-based-gitlab-workflow&owner=%40me&name=skills-release-based-gitlab-workflow&description=My+clone+repository&visibility=public)

1. 右クリックしてコースを開始し、新しいタブでリンクを開きます。
2. 新しいタブでは、ほとんどのプロンプトが自動的に入力されます。
   - 所有者には、個人アカウントまたはリポジトリをホストする組織を選択します。
   - プライベートリポジトリはアクションの時間を使用するため、パブリックリポジトリを作成することをお勧めします。
   - フォームの下部にあるリポジトリを作成ボタンをクリックします。
3. 新しいリポジトリが作成された後、約20秒待ってからページを更新します。新しいリポジトリのREADMEに記載されている手順に従ってください。
