# Guard の使用方法

このプロジェクトでは、Guardを使用してファイルの変更を監視し、テストを自動実行しています。

## インストール済みのGuardプラグイン

- **guard**: コアとなるGuardライブラリ
- **guard-minitest**: Minitestテストの自動実行

## 基本的な使用方法

### 1. Guardの起動

```bash
./bin/bundle exec guard
```

### 2. Guardの停止

Guardが起動している状態で `Ctrl+C` を押すか、`exit` と入力します。

### 3. テストの手動実行

Guardが起動している状態で `Enter` キーを押すと、すべてのテストが実行されます。

## 監視対象のファイル

Guardは以下のファイルの変更を監視しています：

- `app/` ディレクトリ内のRubyファイル
- `test/` ディレクトリ内のテストファイル
- `lib/` ディレクトリ内のRubyファイル

## ファイル変更時の動作

ファイルを変更すると、Guardは自動的に：

1. 変更されたファイルに対応するテストファイルを特定
2. 関連するテストを実行
3. 結果を表示

## 設定ファイル

Guardの設定は `Guardfile` に記述されています。主な設定内容：

- Minitestテストの監視設定
- ファイルパターンの定義
- テスト実行のルール

## トラブルシューティング

### テストが実行されない場合

1. `./bin/bundle install` で依存関係を確認
2. `./bin/rails test` でテストが正常に動作するか確認
3. Guardfileの設定を確認

### パフォーマンスの問題

- 不要なファイルの監視を避ける
- テストファイルの数を最小限に保つ

## 参考リンク

- [Guard公式ドキュメント](https://github.com/guard/guard)
- [guard-minitest](https://github.com/guard/guard-minitest)
- [Rails Testing Guide](https://guides.rubyonrails.org/testing.html)
