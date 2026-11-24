# ThreeMod

ThreeMod は、Three.js を基盤とする AI ネイティブのゲームエンジンです。コードを書かずにゲームやインタラクティブコンテンツを制作できます。

[デスクトップ版のダウンロード](https://github.com/Niceofer/ThreeMod/releases) · [ウェブサイト](https://threemod.com) · [コミュニティ (Discord)](https://discord.gg/uAKu2QjtRP)

[English](./README.md) · [한국어](./README_ko.md)

## 動画で見るThreeMod

| [ひとりでも、ひとつのゲームを完成させる力](https://www.youtube.com/watch?v=r3GPCOFZn9w) | [どんなゲームを作れますか？](https://www.youtube.com/watch?v=pK_qjO2JL0A) |
| :---: | :---: |
| [![ひとりでも、ひとつのゲームを完成させる力](https://i.ytimg.com/vi/r3GPCOFZn9w/hqdefault.jpg)](https://www.youtube.com/watch?v=r3GPCOFZn9w) | [![どんなゲームを作れますか？](https://i.ytimg.com/vi/pK_qjO2JL0A/hqdefault.jpg)](https://www.youtube.com/watch?v=pK_qjO2JL0A) |

[ThreeModのホームページで8つのゲームデモをプレイ](https://threemod.com/?lang=ja#games)

## ダウンロードとインストール

[GitHub Releases](https://github.com/Niceofer/ThreeMod/releases) から、お使いの OS に対応するパッケージをダウンロードしてインストールしてください。

- **Windows**: Windows 用インストーラーを実行します。[Windows インストールガイド](./INSTALL_BYC_WINDOWS.md)も参照してください。
- **macOS**: macOS 用パッケージをダウンロードしてアプリをインストールします。macOS 13 Ventura 以降が必要です。
- **Linux（x64）**: AppImage または `.deb` パッケージをダウンロードしてください。AppImage は実行権限を付与して起動し、Debian/Ubuntu ではパッケージマネージャーで `.deb` パッケージをインストールします。GitHub Actions でのリリース時に Linux ビルドを含めると、Linux 用パッケージも一緒に配布されます。

現在、デスクトップアプリにはコード署名がないため、実行時に OS のセキュリティ警告が表示される場合があります。Windows では **詳細情報 → 実行**、macOS では Finder の **右クリック → 開く**、または **システム設定 → プライバシーとセキュリティ**の実行許可項目を確認してください。

## ブラウザーでの実行例

ThreeMod で制作したコンテンツを、インストールせずにブラウザーでお試しください。

<table>
  <tr>
    <td width="50%" valign="top">
      <a href="https://share.threemod.com/byc_6c536d94e10343adb8a141cff570f990?node=N_LOGI1TO7-NX8XL2Z1"><img src="https://threemod.com/assets/demos/petaflop-duel.gif" width="360" alt=""><br><strong>ペタフロップ・デュエル</strong></a><br>
      <sub>アクション ? ストラテジー ? ターン制</sub>
    </td>
    <td width="50%" valign="top">
      <a href="https://share.threemod.com/byc_6c536d94e10343adb8a141cff570f990?node=N_MLI3AJT1-ZK17KS6J"><img src="https://threemod.com/assets/demos/breaching-the-black-fang-fortress.gif" width="360" alt=""><br><strong>黒牙の要塞突破</strong></a><br>
      <sub>アクション</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://share.threemod.com/byc_6c536d94e10343adb8a141cff570f990?node=N_08PRPK6Y-J5TQJ152"><img src="https://threemod.com/assets/demos/ascent-of-the-wild.gif" width="360" alt=""><br><strong>野生の頂へ</strong></a><br>
      <sub>アクション ? アドベンチャー ? パズル</sub>
    </td>
    <td width="50%" valign="top">
      <a href="https://share.threemod.com/byc_6c536d94e10343adb8a141cff570f990?node=N_YFNFLMWH-1POD7KZ4"><img src="https://threemod.com/assets/demos/nebula-recovery-mission.gif" width="360" alt=""><br><strong>ネビュラ・リカバリーミッション</strong></a><br>
      <sub>アクション</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://share.threemod.com/byc_6c536d94e10343adb8a141cff570f990?node=N_U50BL5HY-06UEZ5PS"><img src="https://threemod.com/assets/demos/a-home-takes-shape.gif" width="360" alt=""><br><strong>家が形になる</strong></a><br>
      <sub>インタラクティブストーリー ? シミュレーション ? 日常</sub>
    </td>
    <td width="50%" valign="top">
      <a href="https://share.threemod.com/byc_6c536d94e10343adb8a141cff570f990?node=N_0KMAK7ZW-ZMCWVR7B"><img src="https://threemod.com/assets/demos/last-stand-against-darkness.gif" width="360" alt=""><br><strong>闇に抗う最後の戦い</strong></a><br>
      <sub>アクション ? ストラテジー ? ファンタジー</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <a href="https://share.threemod.com/byc_6c536d94e10343adb8a141cff570f990?node=N_UGR5ZBG1-KM0W1FMZ"><img src="https://threemod.com/assets/demos/colossus-of-the-arena.gif" width="360" alt=""><br><strong>アリーナの巨像</strong></a><br>
      <sub>アクション ? ファンタジー</sub>
    </td>
    <td width="50%" valign="top">
      <a href="https://share.threemod.com/byc_6c536d94e10343adb8a141cff570f990?node=N_2L3I6QFJ-H6E2NU43"><img src="https://threemod.com/assets/demos/hammerfall-demolition-job.gif" width="360" alt=""><br><strong>ハンマーフォール解体工事</strong></a><br>
      <sub>破壊 ? アクション ? サバイバル</sub>
    </td>
  </tr>
</table>

- [Life Simulation](https://share.threemod.com/byc_f8b97ef4c16045149399d27014556e48)
- [Interaction](https://share.threemod.com/byc_b0cc670cf88f4838b6e1abd80e7755d5)

## リポジトリ構成

- **ルート**: Releases で配布される ThreeMod デスクトップパッケージの紹介、インストール案内、関連資料
- **プレイ用ソース**: 現在配布準備中です。

## 公開する

プロジェクトを自分のサーバーで公開する手順は、プレイ用ソースの配布時に案内する予定です。プレイ用ソースの配布は現在準備中です。

## 利用条件

[ライセンス](./LICENSE.md) · [EULA（英語）](./EULA.md) · [サードパーティーに関する通知](./THIRD-PARTY-LICENSES.md)
