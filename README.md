# DraftEmailReply メール返信案作成
メールの返信案を応対履歴及びメールのテンプレートから生成してくれるソリューションです。

![image](https://github.com/user-attachments/assets/904bb101-bb3d-418e-834a-db41d2ba6ec2)

例えば、コールセンターなどにおける、定型的メールのテンプレートと応対履歴を意識してメール返信案を作成してくれる用途を想定したアプリです。

Dataverse に、「メールのテンプレート」、「応対履歴」を保持ししています。その内容を元に AI がメール返信のドラフトを作成してくれます。

https://github.com/user-attachments/assets/5556c64d-5d2b-4340-94c2-bc29c3726523

そのメールのテンプレートに則って、メールの返信案を作成してくれます。

## 前提条件
* AI Builder を利用しています。そのため、Power Apps Premium ライセンスが必要です。

## ソリューションの利用方法
### インポート方法
[Power Apps の作成者ポータル](https://make.powerapps.com/)に移動します。

[ソリューションのZipファイルはこちら](https://github.com/geekfujiwara/DraftEmailReply/releases/tag/DraftEmailReply)から入手できます。

メニューからソリューションを選択し、インポートを行います。

![image](https://github.com/user-attachments/assets/76996dc5-e062-41d7-9800-99b50a48443d)

ソリューションのZipファイルをインポートします。

![image](https://github.com/user-attachments/assets/c8ec1ee2-e426-45db-b82e-6b337790c303)


> [!note]
> インポートが完了したときに黄色の警告が表示されても問題ありません。表示ラベルに関する警告です。

### メールテンプレートデータ登録
ソリューションに入り、必要なデータを準備します。

データ登録用のモデル駆動型アプリが用意されています。

![image](https://github.com/user-attachments/assets/7578e540-ff4a-4c3f-968a-aaf69d455f2f)

最初にデータを登録する必要があります。メールテンプレートや応対履歴です。

> [!Note]
> 応対履歴はCRMなどから Power Automate コネクターを経由してデータを連携するのもよいかと思います。

[モデル駆動型アプリ](https://learn.microsoft.com/ja-jp/power-apps/maker/model-driven-apps/build-first-model-driven-app)にて、メールテンプレートの登録を行うことが出来ます。

![image](https://github.com/user-attachments/assets/5609e443-d11c-41aa-946b-ad0933303f90)

モデル駆動型アプリではExcel Onlineから一括でデータを登録することも出来ます。

![image](https://github.com/user-attachments/assets/b62e04fc-10df-4704-9f20-4efc9c3c0149)

Excel Online を選択します。

![image](https://github.com/user-attachments/assets/33131c33-fb06-4f03-984c-c079733d3304)

こちらから一括でメールテンプレートのデータを登録してください。

![image](https://github.com/user-attachments/assets/087f9ef3-5051-4747-8ea0-3a4c95557b51)

> [!Note]
> 同じように応対履歴を登録することが出来ます。

以上、ご参考になれば幸いです。


