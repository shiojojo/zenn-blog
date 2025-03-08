---
title: "Mailtrapを利用した開発環境でのメール送信テスト"
emoji: "📝"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: [メール実装, Mailtrap, 開発環境, テスト, メール送信]
published: true
---

# 概要
本記事では、開発環境でメール送信のテストを行う際の課題とその対策について解説します。  
実際のメール送信では、セキュリティポリシーの制限や誤認識により、コードの問題か環境依存の問題か判断が難しくなるケースがあります。  
そこで、Mailtrapを利用して安全かつ正確にテストメールの送信状況を確認する手順を紹介します。

# Mailtrapの紹介
Mailtrapは、テスト用のメールアドレス（例: *@example.com*）を利用できるサービスです。  
- 料金：無料  
- クレジットカード登録：不要  

※料金は変更される可能性があるため、使用前に以下を確認してください。
https://mailtrap.io/pricing/


# Mailtrapの利用手順
以下の手順でMailtrapへの登録とテストメール送信の確認を行います。

1. **サインアップ**
   - [Mailtrap](https://mailtrap.io/) にアクセスし、右上の「サインアップ」をクリックします。

2. **ユーザー情報の登録**
   - 名前など必要情報を入力します。  
   ![manual-01](/images/develop-send-mail/manual-01.png =600x400)

3. **利用用途の選択**
   - ここでは「テスト用」として利用する項目にチェックを入れます。  
   ![manual-02](/images/develop-send-mail/manual-02.png =600x400)

4. **メールボックスの確認**
   - 登録完了後、「My Inbox」というメールボックスが自動で作成されます。  
   ![manual-03](/images/develop-send-mail/manual-03.png =600x400)

5. **メール送信先と関連情報の確認**
   - 「My Inbox」をクリックすると、送信先メールアドレスおよびその他の必要な情報が表示されます。  
   ![manual-04](/images/develop-send-mail/manual-04.png =600x400)

6. **送信コードの確認**
   - ページ下部に、実際のメール送信に使用するコード例が表示されます。  
   ![manual-05](/images/develop-send-mail/manual-05.png =600x400)

7. **テストメール送信**
   - ここでは、パスワードリセットメールを例としてテストメール送信の動作を確認します。
   - テストメール送信後、以下のようにメールが受信され、実装が正しく動作していることを確認できます。  
     送信元および送信先のアドレスには、`@example.com` を使用しています。
     
   ![manual-06](/images/develop-send-mail/manual-06.png =600x400)


