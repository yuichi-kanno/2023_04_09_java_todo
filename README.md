SpringBootのファイル名の役割
一部はあくまでこのファイル内での役割を記載している部分もあります。


### MVCとは
Model:主にデータベースとのデータのやりとりを行う
View:ユーザーとWebサイトとのインターフェイス。画面表示。
COntroller:ModelとViewの橋渡し。

### @Controllerとは
classの上部に@controllerというアノテーションを付与すると、SpringBoot側がそのクラスを Controller として認識する。
serviceクラスで定義したメソッドを実行してViewへ接続する。

### @RequestMappingとは
@RequestMappingというアノテーションを付与すると、クライアントからのリクエストに対してメソッドやハンドラをマッピングします
@GetMapping、@PostMappingなどをメソッドに付与すると、それぞれGETリクエスト、POSTリクエスト処理時に実行される。

### Entityとは
DBのレコードを表現するJavaクラス。
ここで定義したClassの型をDaoクラスのメソッドの引数に渡したりする。

### @Repositoryとは
データ層のクラスに付与する。  
DAOなどのDBアクセスを行うクラスに付与するのが一般的。

### @Serviceとは
サービス層のクラス（ビジネスロジック等）に付与する。
Service は業務処理を提供する。クラスが DI コンテナへの登録対象としてマークされます。
Daoクラスで定義したメソッドを実行するメソッドを定義したりする。

### @AutoWiredとは
DI コンテナへ登録されたインスタンスを注入したい箇所に設定します。



参考：https://yo1000.gitbooks.io/self-study-spring/content/

