# EF03_Order_結合試験項目書

## EF0301-UC01-T01_カート（[お買い物を続ける]ボタン押下）

1. TOPページ(ログアウト状態)→商品一覧→商品詳細
1. 数量1を入力し「カートに入れる」ボタンを押下する
1. 「カートに進む」ボタンを押下する
1. ショッピングカート画面に遷移する
1. [お買い物を続ける]ボタンを押下
1. TOP画面に遷移する

## EF0301-UC01-T02_カート（[✕]ボタン押下）

1. TOPページ(ログアウト状態)→商品一覧
1. 数量1を入力し「カートに入れる」ボタンを押下する
1. 「お買い物を続ける」ボタンを押下する
1. 異なる商品かつ、数量１を入力し「カートに入れる」ボタンを押下する
1. 「カートに進む」ボタンを押下する
1. ショッピングカート画面に遷移する
1. カートに入れた２商品が一覧表示される
1. 合計が正しく計算されている
1. [✕]ボタンを押下する
1. 削除確認のダイアログが表示される
1. OKを押下する
1. 対象の商品が一覧から消え、商品数、合計金額が再計算される。

## EF0301-UC01-T03_カート（数量の変更）

1. TOPページ(ログアウト状態)→商品一覧→商品詳細
1. 数量1を入力し「カートに入れる」ボタンを押下する
1. 「カートに進む」ボタンを押下する
1. ショッピングカート画面に遷移する
1. [＋]ボタンを押下する
1. 対象の商品の商品数が2となり、合計金額が再計算される。
1. [-]ボタンを押下する
1. 対象の商品の数量が1となり、合計金額が再計算される。

## EF0301-UC01-T04_複数ブラウザでのカート操作

1. ブラウザAで、会員ログインを行う
1. ブラウザBで、会員ログインを行う
1. ブラウザAで、商品をカートに入れ、カート画面を表示する
1. ブラウザBで、カート画面を表示し、ブラウザAで投入した商品が表示されることを確認する

## EF0301-UC01-T05_複数ブラウザでのカート操作

1. ブラウザAで、会員ログインを行う
1. ブラウザAで、商品をカートに入れ、カート画面を表示する
1. ブラウザBで、商品をカートに入れる
1. ブラウザBで、会員ログインを行う
1. ブラウザBで、カート画面を表示する
    1. ブラウザAとBで投入された商品がマージされ、カートに表示されることを確認する
1. ブラウザAで、カート画面を表示する
    1. ブラウザAとBで投入された商品がマージされ、カートに表示されることを確認する

## EF0302-UC01-T01_ログインユーザ購入（通常パターン）

1. TOPページ(ログアウト状態)→商品一覧→商品詳細
1. 数量1を入力し「カートに入れる」ボタンを押下する
1. 「カートに進む」ボタンを押下する
1. ショッピングカート画面に遷移する
1. [レジに進む]ボタンを押下する
1. ログイン/ゲスト購入選択画面が表示される
1. メールアドレス/パスワードを記入する
1. [ログイン]ボタンを押下する
1. ご注文手続き画面が表示される
1. お客様情報、配送情報、お支払方法、利用ポイント、お問い合わせ、小計・手数料・送料・値引き・合計・ご利用ポイント・加算ポイントに正しい情報が表示されていることを確認する
1. [確認する]ボタンを押下する
1. ご注文内容のご確認画面に遷移する
1. ご注文手続き画面で入力した内容が表示されている
1. [注文する]ボタンを押下する
1. 注文完了画面が表示される
1. 注文完了メールが送信される
1. [トップページへ]ボタンを押下
1. トップページが表示される。

## EF0302-UC02-T01_ゲスト購入（通常パターン）

1. TOPページ(ログアウト状態)→商品一覧→商品詳細
1. 数量1を入力し「カートに入れる」ボタンを押下する
1. 「カートに進む」ボタンを押下する
1. ショッピングカート画面に遷移する
1. [レジに進む]ボタンを押下する
1. ログイン/ゲスト購入選択画面が表示される
1. [ゲスト購入]ボタンを押下
1. お客様情報の入力画面が表示される
1. お客様情報フォームを入力する
1. [次へ]ボタンを押下
1. ご注文手続き画面が表示される
1. お客様情報、配送情報、お支払方法、利用ポイント、お問い合わせ、小計・手数料・送料・値引き・合計・ご利用ポイント・加算ポイントに正しい情報が表示されていることを確認する
1. [確認する]ボタンを押下する
1. ご注文内容のご確認画面に遷移する
1. ご注文手続き画面で入力した内容が表示されている
1. [注文する]ボタンを押下する
1. 注文完了画面が表示される
1. 注文完了メールが送信される
1. [トップページへ]ボタンを押下
1. トップページが表示される。

## EF0303-UC01-T01_ログイン/ゲスト購入選択画面でログイン時,販売種別が異なる商品がカートに入っている場合、ご注文手続き画面ではなくショッピングカート画面に戻す

1. TOPページ(ログイン状態)→商品一覧→商品詳細
1. 販売種別Aの商品をカートに入れる
1. ご注文手続き画面にすすむ
1. 購入せずにログアウトする
1. 販売種別Bの商品をカートに入れる
1. [レジに進む]ボタンを押下する
1. ログイン/ゲスト購入選択画面が表示される
1. メールアドレス/パスワードを記入する
1. [ログイン]ボタンを押下する
1. ショッピングカート画面に遷移する
1. 「同時購入できない商品がカートに含まれています。」が表示される
1. カートが複数に分かれる

## EF0305-UC02-T01_ゲスト購入（お客様情報の変更）

1. TOPページ(ログアウト状態)→商品一覧→商品詳細→カート
1. TOPページ>商品一覧>商品詳細>カートへ遷移
1. [レジに進む]ボタンを押下
1. ログイン/ゲスト購入選択画面が表示される
1. [ゲスト購入]ボタンを押下
1. お客様情報の入力画面が表示される
1. お客様情報フォームを入力する
1. [次へ]ボタンを押下
1. ご注文内容のご確認画面が表示される
1. 注文明細、小計・手数料・送料・合計、お客様情報、お届先情報、お支払い方法、お問い合わせ欄に正しい情報が表示されていることを確認する
1. お客様情報セクションの[変更]ボタンを押下する
1. お客様情報が全て編集可能となる。
1. お客様情報セクションの入力フォームの値を変更する
1. [OK]ボタンを押下する。
1. [確認する]ボタンを押下する
1. ご注文内容のご確認画面に遷移する
1. ご注文手続き画面で入力した内容が表示されている
1. [注文する]ボタンを押下
1. 注文完了画面が表示される
1. 注文完了メールが送信される
1. [トップページへ]ボタンを押下
1. トップページが表示される。

## EF0305-UC04-T01_ゲスト購入（お届け先情報の変更）

1. ゲスト購入でご注文手続き画面に遷移する
1. 配送情報セクションの[変更]ボタンを押下する
1. お届け先の変更画面へ遷移する
1. お届け先情報フォームを編集する
1. [登録する]ボタンを押下する
1. ご注文手続き画面に遷移する
1. 配送情報が更新されていることを確認する

## EF0305-UC04-T02_ゲスト購入（お届け先情報の追加）

1. ゲスト購入でご注文手続き画面に遷移する
1. 同じ商品種別の商品を２つカートに入れ、ご注文手続き画面に遷移する
1. [お届け先を追加する]を押下し、お届け先の複数指定画面に遷移する
1. [新規お届け先を追加する]ボタンを押下し、お届け先の追加画面に遷移する
1. お届け先情報フォームを入力する
1. [登録する]ボタンを押下し、お届け先の複数指定に遷移する
1. お届け先のプルダウンで登録した配送先を選択する
1. [選択したお届け先に送る]ボタンを押下し、ご注文手続き画面に遷移する
1. お届け先が更新されていることを確認する

## EF0305-UC04-T03_ゲスト購入（お客様情報の変更→お届け先情報の追加）

*https://github.com/EC-CUBE/ec-cube/issues/5229 のリグレッションテスト*

1. 同じ商品種別の商品を２つカートに入れ、ご注文手続き画面に遷移する
1. お客様情報セクションの[変更]ボタンを押下する
1. お客様情報が全て編集可能となる。
1. お客様情報セクションの入力フォームの値を変更する
1. [OK]ボタンを押下する。
1. [お届け先を追加する]を押下し、お届け先の複数指定画面に遷移する
1. [新規お届け先を追加する]ボタンを押下し、お届け先の追加画面に遷移する
1. お届け先情報フォームを入力する
1. [登録する]ボタンを押下し、お届け先の複数指定に遷移する
1. お届け先のプルダウンで登録した配送先を選択する
1. [選択したお届け先に送る]ボタンを押下し、ご注文手続き画面に遷移する
1. お届け先が更新されていることを確認する

## EF0305-UC05-T01_お届け先の追加

1. ログイン後、商品をカートに入れ、ご注文手続き画面に遷移する
1. 配送情報セクションの[お届け先を追加する]ボタンを押下する
1. お届け先の指定画面へ遷移する
1. [新規お届け先を追加する]ボタンを押下する
1. お届け先情報フォームへ遷移する
1. お届け先の追加フォームを入力し、[登録する]ボタンを押下する
1. お届け先の指定画面へ遷移する
1. [お届け先追加]ボタンを押下する
1. お届け先と数量を編集する
1. [選択したお届け先に送る]ボタンを押下する
1. ご注文手続き画面に遷移する
1. 配送情報が更新されていることを確認する

## EF0305-UC06-T01_複数配送 - 同じ商品種別

1. 同じ商品種別の２つ商品をカートに入れ、ご注文手続き画面に遷移する
1. 配送情報セクションの[お届け先を追加する]ボタンを押下する
1. お届け先の指定画面へ遷移する
1. 2つ同じお届け先を設定する
1. [選択したお届け先に送る]ボタンを押下する
1. ご注文手続き画面に遷移する
1. 2商品が１つの届け先に設定される

## EF0305-UC06-T02_複数配送 - 同じ商品種別

1. 同じ商品種別の２つ商品をカートに入れ、ご注文手続き画面に遷移する
1. 配送情報セクションの[お届け先を追加する]ボタンを押下する
1. お届け先の指定画面へ遷移する
1. 2商品を異なるお届け先を設定する
1. [選択したお届け先に送る]ボタンを押下する
1. ご注文手続き画面に遷移する
1. 2商品が別々のお届け先に設定される

## EF0305-UC06-T05_複数配送 - 注文確認戻る

前提：  
お届け日：商品もしくは規格で発送日目安を設定しておく  
お届け時間：設定→店舗設定→配送方法設定 で任意の配送業者名リンクをクリックして設定しておく

1. 同じ商品種別の２つ商品をカートに入れ、ご注文手続き画面に遷移する
1. 配送方法、お届け日、お届け時間を設定する。
1. [お届け先を追加する]を押下する。
1. 戻るボタンを押下し、ご注文手続き画面に遷移する
1. 配送方法、お届け日、お届け時間の設定内容を保持して表示する

## EF0305-UC06-T06_複数配送 - 更新

1. 同じ商品種別の商品を２つカートに入れ、ご注文手続き画面に遷移する
1. [お届け先を追加する]を押下し、お届け先の複数指定画面に遷移する
1. [新規お届け先を追加する]ボタンを押下し、お届け先の追加画面に遷移する
1. お届け先情報フォームを入力する
1. [登録する]ボタンを押下し、お届け先の複数指定に遷移する
1. お届け先のプルダウンで登録した配送先を選択する
1. [選択したお届け先に送る]ボタンを押下し、ご注文手続き画面に遷移する
1. お届け先が更新されていることを確認する

## EF0305-UC06-T07_販売種別が一致しないケース

1. 異なる商品種別の２つ商品をカートに入れ、ショッピングカート画面に遷移する
1. 「同時購入できない商品がカートに含まれています。」のメッセージが表示される
1. ショッピングカートが２つに分かれる

## EF0305-UC07-T01_複数配送 - ログインしてカートをマージ

1. ログイン後、１つの商品をカートに入れ、ご注文手続き画面に遷移する
1. ログアウトする
1. 同じ販売種別の別の商品をカートに入れ、ログイン/ゲスト購入選択画面に進む
1. 先程ログインしていたユーザーのメールアドレス/パスワードを入力し、[ログイン]ボタンを押下する
1. ご注文手続き画面に遷移する
1. 以前ログイン中だった注文明細が表示されている。

## EF0305-UC08-T01_複数配送 - 購入確認画面からカートに戻る

1. 同じ商品種別の商品を２つカートに入れ、ご注文手続き画面に遷移する
1. 配送方法、お届け日、お届け時間、お支払い方法を設定する。
1. [カートへ戻る]ボタンを押下する
1. [レジに進む]ボタンを押下する
1. 設定したお届け先が復元される(ただし、配送方法を変更したあとにお届け日とお届け時間を変更した場合は値は保持されておらず復元されない)

## EF0305-UC08-T02_複数配送 - 購入確認画面からカートに戻る(お届け先初期化)

1. 同じ商品種別の商品を２つカートに入れ、ご注文手続き画面に遷移する
1. 配送方法、お届け日、お届け時間、お支払い方法を設定する。
1. [お届け先を追加する]を押下する。
1. 新しいお届け先を追加する
1. [選択したお届け先に送る]ボタンを押下し、ご注文手続き画面に遷移する
1. 以上の設定したお届け先が設定されている。(ただし、配送方法を変更したあとにお届け日とお届け時間を変更した場合は値は保持されておらず復元されない)
1. [カートに戻る]ボタンを押下
1. 新しく商品をカートに追加する
1. [レジに進む]ボタンを押下
1. お届け先が初期化される

## EF0305-UC09-T03_複数配送 - 複数配送設定画面での販売制限エラー

1. TOPページ→販売制限数が5の商品を5つカートに入れて、ご注文手続き画面に遷移する
1. [お届け先を追加する]を押下し、お届け先の複数指定画面に遷移する
1. [お届け先追加]ボタンを押下し、1つ目のお届け先は数量2、2つ目のお届け先は数量4に設定する
1. [選択したお届け先に送る]ボタンを押下し、ご注文手続き画面に遷移する
1. 販売制限についてのメッセージが表示される
1. お届け先(1)の数量が2となる
1. お届け先(2)の数量が3となる
