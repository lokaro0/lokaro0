# Software Engineering Portfolio

コンピュータ科学と機械学習を学んでいます。
C++を中心としたソフトウェア開発、ゲームシステム、AIに関心があり、動くものを作るだけでなく、設計・テストまで含めて改善することを重視しています。

## Featured Project

### [Falling Puzzle Game](https://github.com/lokaro0/falling-puzzle-game)

`C++17` `raylib` `ncurses` `CMake` `CTest` `GitHub Actions` `Git` `Windows / WSL / Ubuntu`

2個組の色付きピースを操作し、同色のピースを4個以上つなげて消す落下パズルゲームです。Windows向けのraylib GUI版と、Linux／WSL向けのncurses版を公開しています。

[Windows版をダウンロード（v0.3.0-preview）](https://github.com/lokaro0/falling-puzzle-game/releases/tag/v0.3.0-preview)

Windows版はZIPを展開して起動できます。タイトル・プレイ・結果・再挑戦の画面遷移、連鎖と同時消しの得点計算、点滅・連鎖表示、効果音、ハイスコア保存を実装しました。

<img src="https://raw.githubusercontent.com/lokaro0/falling-puzzle-game/main/assets/gui-gameplay.png" alt="Falling Puzzle GameのWindows GUI版プレイ画面" width="500">

- ピースの生成・移動・回転・着地、盤面管理、連結探索、消去、重力、連鎖、スコアを実装
- 単一ファイルだった初版を、`domain`・`ui`・`storage`へ責務分離
- 手動メモリ管理を`std::vector`へ置き換え、ncursesセッションをRAIIで管理
- 盤面、ピース、ゲームルール、ハイスコア保存の4系統をCTestで自動検証
- CMakeを使い、WSL／Ubuntu上で再現可能なビルド手順を整備
- README、アーキテクチャ資料、リファクタリング記録を公開

GitHub Actionsの対象はUbuntuでのncurses版ビルドと共通ロジック・保存処理のテストです。Windows GUIの画面や音の検証は含みません。

## Team Project

### Kagami Mochi Game App

`Dart` `Flutter` `Riverpod` `Team Development`

5人で制作した鏡餅をテーマとするゲームアプリで、図鑑・運勢表示機能を担当しました。

- 鏡餅の素材と完成形を表すデータモデルを定義
- enumを使って餅・果物・台座の素材データを管理
- 3×3×3の全27通りについて、名称・運勢・解説文を生成するロジックを実装
- Riverpodで管理される既存の選択状態を参照し、図鑑一覧、詳細ダイアログ、運勢表示、画面遷移へ統合

## Technical Skills

| Area | Skills |
| --- | --- |
| Languages | C++, C, Python, Dart |
| Development | Data structures, game loops, state management, file I/O, automated testing |
| Tools / Environment | Git, GitHub, GitHub Actions, CMake, Linux, WSL, Visual Studio Code |

## Current Focus

- C++による設計・実装・テストの経験を深める
- 機械学習をライブラリの利用だけでなく、アルゴリズムの原理から理解する
- ゲームAI、ゲームエンジン、性能を意識したソフトウェア開発へつながる基礎を身につける

## Links

- [GitHub](https://github.com/lokaro0)
- [Falling Puzzle Game](https://github.com/lokaro0/falling-puzzle-game)
