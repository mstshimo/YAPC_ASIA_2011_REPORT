YAPC::Asia Tokyo 2011
場所:東京工業大学 大岡山キャンパス

日時:10月13日(木) 前夜祭(予定)
     10月14日(金) 一日目
     10月15日(土) 二日目


まとめ：
今年は、2回目の参加となった。前夜祭にも参加した。
昨年はなるべく英語の公演は避けたが、
今年は、英語でも興味のあるワードが並んでいるもの聞いてみることにした。
自分には内容が難しかったのか、セッション内容が分からないものもあったが、
なんとなく分かるセッションもあり、聞いて良かった。
今年は、YAPC Tシャツの当日販売がなくて、購入できなかったのが残念でした。
また、シャツもサイズが品切れで購入できなかった。

新しく聞いたワード:
Carton
Qudo
DevOps
EMAIL::SIMPLE
EMAIL:MESSAGE
XML::Atom::Clinets;
XML::Atom::Entry;
Net::OpenID::Consumer
Padre
Mi
Test::Mysqld
Test::Fixture::DBI
Scope::Container
Scope::Container::DBI

==================================================================
Opening [ja] [any][community]
941
10:30-10:50
==================================================================
記録
	過去最大参加者
	過去最大トーク申し込み
	過去最大スポンサー
	東工大のプロジェクタが変わったが、使えず結局購入した12万のプロジェクターを使った。
	LEDの照明に変わった。
	71のトーク申し込み例年の1.5

新たな試み
	遠方参加者支援…SKYARC Ssystem
	個人スポンサー 約90名
	スイーツエリア設置


YAPCの楽しみ方
	１．トークを聞こう
	２．YAPCスポンサーと企業の方々と交流しよう
	３．PerlHackerと交流しよう
	４．投票しよう

ゲスト紹介
Guest Speakers
	Ricardo Signes
	Marc Lehmann
	木村 秀夫

Special Guests
	宮川達彦
	Jesse Vincent

==================================================================
Perl 5.16 and beyond [en] [any][library]
Jesse Vincent
11:00-11:30
==================================================================
Perl6の元プロジェクトマネージャー

Perl5のパンプキン・・・・決断する人

誰がPerlを作っている？CPAN Author?
	皆さんがPerlを作っている

Perlのルール
	ルール1
		ラリーが全て正しい
	ルール2
		ラリーが後から考えが変わっても良い

	このルールはラリーだけでも、パンプキンだけでもない
	Perlはいつも正しい
	考えを変えても正しい

今の最新版 v5.14.2
	昔は１つのリリースに3週間掛かったが、今は１日も掛からない
	新しいコミッタ
	リリースにはコミット権が必要
	gitにしてから増えた

リリースが簡単になった、今だから言えるPerl5のビジョン
	新しいバージョンを出しても、既存を壊さない
	古い文法や挙動を守るために成長をあきらめない

	間違うこともあるかもしれない。実際あった。
	間違ったら正せるようにしなけれならない
	去年のまともなデフォルトも正せなければならない
	Perl5はもっとPerl5で
	あらゆるところで実行できなくては

use v5.16;
	これからは欲しいバージョンを呼ぶ
	古いバージョンを求められたら、新しい機能は動かないように
	既存のコードを壊すのは最後の手段
	大変だけど、できないことではない。

機能の廃止サイクル
	廃止のサイクルは今は1年になっている

ルール2と古いモジュールについて
	Perlは大きな言語、もっと大きな言語もあるけど、言語が大きくなると大変
	バグも取るのも大変
	コアの開発チームは良くやってるけど、すごくはない
	しかし、コミュニティーはすごい

言語を小さくするには？
	言語レベルでもサポートする必要のないものもある。
	廃止するわけでなく、言語レベルのサポートから外すだけ

SysV実装はモジュールでも良いだろう
将来的にhモジュール化してバグを直すかも

use 5.12でuse strict される。

2引数のopenはデフォルトでは消す
オブジェクトの間接記法を無効にする


==================================================================
Carton: CPAN dependencies manager [ja] [beginner][library]
Tatsuhiko Miyagawa
12:00-11:20
==================================================================

依存関係がわからない
システムに入ってるPerlでマシンで違う

MyCPAN, DPAN, OrePAN
基本的にtarballでばらまく

気に入らないので、自分で書いてみた。
	Cartonと言う・
	RubyのBundlerをinspire

Local perl environment
	システムにデフォルトで入っているPerlではなく、ローカルに

Fast and safe install
	環境が分かれるので安全だし、高速

Dependence tree analytics
	依存ツリーの解析

Locking versions
	全バージョンの固定

Single-file, VCS friendry
	JSONの1ファイルで管理してるが、変更するかも

Demo
DancerインストールをCartonを使いデモ

IRC
	server:perl.org
	channel:#carton


==============================================================
SmartPhone development guide with Node/CoffeeScript 
and HTML5 technologies, for Perl programmers [ja] [any][app]
Naoya Ito
12:20-12:40
==============================================================

PhoneGap
	HTML+CSS+Javascriptを書いてアプリをつくる

Titanium Mobile
	jsで書いてアプリをつくる

HBFav
	はてなブックマークお気に入りリーダー

	js
	CoffeeScript
	Herok

SL4A
	perlでクライアントサイド、まだ。。。


クライアントをjsで書いたら、サーバサイドもっていう流れば止められない

Node.js
	Perl::POE, AnyEvent

search.npmjs.org
	CPANみたいなもの

undersocre.js
	Express シナトラにinspire

Test::Declar
VOWS

xml2js

aws-lib…アマゾンAPIを使える

Socket.IO
	WebSocket like API

pocketio
	PerlのSocketIOサーバ

・スマートフォン：今後ネイティブからHTML5で
・jsのみでクライアントアプリが
・Node.js

※凄く早口で、頭が追いつかなかった

==============================================================
AnyEvent, Coro, IO::AIO - a good team [en] [intermediate][library]
Marc Lehmann
13:40-14:20
==============================================================
内容も難しかったのか、良くわからなかった。




==============================================================
perlbrew [en] [beginner][library]
Kang-min Liu
14:40-15:00
==============================================================
perlのバージョンupをすると@INCが長くなる

rvm…ruby
perlbrew･･･perl

installation 
	curl -kL http://xrl.us/perlbrewinstall | bash

	perlbrew install 5.14.2
	perlbrew install perl-5.8.1
	perlbrew install perl-5.13.6

use 
	perlbrew use perl-5.14.2
	perlbrew list

usage
	perlbrew lib list

benefits
	sudo cpanをする必要がもやはなくなった
	perl-appの分離した環境構築

http://www.perlbrew.pl/


==============================================================
Perl 5.14 For Pragmatists [en] [any][library]
Ricardo Signes
15:00-15:40
==============================================================
Perl 5.14
	5.10は大きな変更があった
	5.12は少し小さい

「:=」
sub login : local {..}
my $x : Private = 10;
my $x := 10;

「qw()」


s///r
「r」
新しい正規表現の修飾子
my @short_names = 
	map {
		s/\..*//r
	} @long_names

eachにarray refが使える？

use 5.14.0;
use autodie;

$@について
	Try::Tiny;

IPv6 Support!

say "I \23145 Perl 5.41!";


==============================================================
他言語から見たPerlのテスト [ja] [any][testing]
Masaki Nakagawa
16:00-16:20
==============================================================
組み込み開発
	ハードウェアドリブン
	ウォータフォールになりがち
	しかし、テストは体型的になっている
	テストの分類をしっかりしてないと何をやってるかわからなくなる

分類の仕方
	テストの視点
	テストをする人は誰か？
	開発者 Test
	ユーザ Test

テストの対象
	Unit(単数)
	Integration(複数)

テスト手段
	BlackBox
	WhiteBox

テスト目的
	FuntionTesting
	Non-Functional Testing
		Perfomance

Testing Frameworkやってるくれること３つ
	Helping to write tests
	Executeing test
	Repoting Test

Ruby Testing
TestUnit

RScpec・・書き方に特徴
describe なんのテストかを書く
it テストを書く

Cucumber…受け入れテスト用
given when then


Perlの場合
	Test::More
	Test::Class
	xUnit like

Test::Base
	データの繰り返し

Test::Spec

Perl has TAP
	PerlのテストはTAPを抜きにはできない
	Tapに合わせた形にするような使われた方

Tap::Formatter::Junit

PerlはTAPを使うことにより拡張性を持たしている

RailesTesting
Railes3

UnitTest, End-to-End(ブラウザin out)
	RSpec, Cucumber

Browser Integration
	Capybara(一番有名みたい)

Test Duble
WebMock
rr(ダブルルビーと読む)

Catalyst
CatalystTets
Test::WWW::Mechanize::Catalyst
Test::WWW::Selenium::Catalyst

Plack
Plack::Test

Mock
	Test::MockObject

Stub
	Test::MockGurd

Test Double

Spy
DBD::Mock

Stubしかないのに、モックと呼ばれるのが気になる

TAPベースなので、沢山のモジュール（やり方)がある
ブラウザインテグレーションは弱い
ベリフィケーションが弱い。
→tokuhiromuさん、、、なんのことを指していますか？
→メソッドなどが何回呼ばれたか
→test planで可能なのでは？
→test planはテストの数なので。
→なるほど。

========================================================
Apporoで類似文字列検索 [ja] [any][library]
Toshinori Satou
16:20-16:40
========================================================
@overlast
類似文字列検索エンジン Apporoの応用とお題を変更

PerlからC/C++へスケールしている

Apporoの概要
	お手軽で高速な類似文字列検索をしたい

Googleサジェストみたいなもの
辞書メンテナンスのコスト
表記バリエーションを手でメンテするのはありえない。

開発言語C++(Perl拡張を用意)

競合Product
Apache Lucene
SimString


======================================================
LT Day 1 [ja] [any][other]
17:00-
======================================================
--------------------------------------
@makamaka
--------------------------------------
「同人誌活動報告」

Acme大全2011
	用語集も含めより詳しく。
	逆引き時点も付いている。

Perlのカードゲーム

※DeNAなどで、PerlMongerゲームみたいない感じで流行らせたら？ｗ
と個人的に思った。

--------------------------------------
@tokuhirom
--------------------------------------
「Amon2 3.0」
	WAF

--------------------------------------
@hakobe932
--------------------------------------
「Enhance Anime wathing with programing」

アニメ情報を出すアプリを作った

※個人的に面白度が高いなぁと思った

--------------------------------------
スポンサーセション KAYAC
荒井けんさく
--------------------------------------
「Perl道場」リリース

PHPer、カヤックにてPerlに入門、しかしJSを書いている
Perl道場をリリースした
http://perldojo.org/

--------------------------------------
@yappo
--------------------------------------
「App::Ikachan」

みんなIRCを使ってますよね。
IRCボットをWebから？
ikachan

--------------------------------------
@kenich
--------------------------------------
「Let's play games」

倉庫番ゲーム

--------------------------------------
@egopro
--------------------------------------
「仙台で1年間PMをやってみた」

Sendai.pmが登録された

sendai.pm.org
@sendaipm

準備室が取れ、Sendai.pm#1を予定

--------------------------------------
スポンサーセッション SKYARC System
@onagatani
--------------------------------------
「北海道のIT勉強会事情の紹介」

MTの仕事をしている

北海道PMを開催したい
Rubyもやってるから出来るはず

--------------------------------------
@issm
岩田淳
--------------------------------------
「ようやく始まりましたNagoya.pm」

nagoya.pm

名古屋の良さを紹介

11/20#2予定

--------------------------------------
@mayumin
--------------------------------------
「Perlが決める未来」

Six Apartの方
Perlデビューして1週間で、Siriをinspireして、ブラウザとの会話アプリ
コードはGithubに有るとのことだが、YAPCが終わったら削除予定、
といってたので、無いかも。

--------------------------------------
@kanper さとうけんた
--------------------------------------
「アクセサについての考察」

アクセサについて考察してみる

Class::VirtualAccessorの紹介？

--------------------------------------
@turugina
--------------------------------------
「日常業務でperlを使おう」

webタイムカード？

--------------------------------------
リクルート
--------------------------------------
「マッシュアップアワード7」

現在90作品

Ninja Challenge

36時間耐久ハッカソンを予定

--------------------------------------
JPA 岡部恵一
--------------------------------------
「Perl商標の話」

Perlを関係ない人が商標登録したらしく、それを奪還するまでの話。
5minの無視の、とても重要な話だった。

--------------------------------------
@keroyonn_
--------------------------------------
「Perlで次世代ゲーム開発」

cuiゲーム

※昨年、Tatsumakiのセッションをやった方だと懇親会で気がついた。


--------------------------------------
@arisawa
--------------------------------------
「ぼくたちのPerl Module管理」

darkpan
	CAPNの部分ミラー

OrePAN
	CPANの部分ミラーを作るもの

--------------------------------------
@nekokaku
--------------------------------------
「not ORM - for @kamipo」

perlO/R
DBIx::Class
DBIx::Skinny
DBIx::TransactionManager
DBIx::Connector
SQL::Object
DBIx::Handler

--------------------------------------
@tagomoris
--------------------------------------
ISUCON
	webアプリ高速化祭り

優勝はkAYACの方がしたみたい
livedoor techblogにコードがある。


======================================================
懇親会
======================================================


======================================================
続 Unix Programming with Perl [ja] [intermediate][tutorial]
Kazuho Oku
======================================================
昨年のファイルハンドル、シグナルについての続編的な話。

シグナルのレースコンディション？
inter-process？

Writing correct code
PerlとOSの知識を持って正しいコードを書く

$! and Errno

file handoles

Unix signals

inter-process

IPC::Open3-Pipe and Deadlock
ブロックする可能性があるのどこなのか？

一方でデータ入力待ち、一方はプロセス終了待ち
→入力プロセスは閉じる。


Pipe has size limit
64Kbyte linux
16Kbyte Mac

TCPストリームやTCPソケットにもある。

パイプを使わずに、テンポラリのファイルに書き込む
なぜ、リダイレクトを使わないのか？
シェル呼び出しを避けるため。

POSIX::pselect

use system @args or IPC::Open3

非同期処理、Any::Eventであればこの辺は問題にならないと思う。

※難しくて分からない。

======================================================
運用しやすいWebアプリケーションの構築方法 [ja] [intermediate][app]
masahiro nagano
@kazeburo livedoor
11:00-11:40
======================================================
1億PVから10億PVへのスケールアプト
罠がある→運用ノウハウを広める

運用しやすい
	
障害を起こさない
→耐障害性

早い復旧

スケーラビリティ

Log::Minimal
	アプリケーションからの情報発信
	障害の際に最初に見る
	障害の検知

strace -p PID/gdb -p PID
アクセスログ
バイナリログ

良いログモジュール/良いログとは？
適切なログに含まれる情報
・時間
・ログレベル
・環境(PID,uri,引数)
・caller/stacktrace
・読み取る人に伝わるメッセージ


Log::Minimal okuさんが作成
Log::Dispatchなぜ作られたか理解できない、拡張しやすい？

DBの負荷
・原因となっているクエリを探す
・何のクエリなのかアプリケーションのコードを確認
killしていいのか？
クエリチューニング

ORMきらい
SQLとクエリが一致しない

SQLを生成するモジュールが散らばらないで欲しい
クエリのコメントに情報があると良い

DBIx::Sunny
DBI(connection)

接続の滞留

Scope::Container
Scope::Container::DBI


cache/memchached
特定キュッシュへの集中
Cache thundering herd problem

キャッシュのヒットがなくなると一気にDBへアクセスして死ぬ

use Metrics;

※後半、難しかった。

======================================================
watch your log [ja] [intermediate][infra]
nekokak
12:00-12:40
======================================================

DBIx::Skinny
	Teng
Qudo


状況に応じた、必要なエンジニアリングをしよう


DevOps

運用を考えられるDevとは？
	何かしら障害が発生した場合、多くはOpsの人が一次対応を行うはず。
	一時対応が行える共有をすべき

丸受けしないOpsとは？
	サービス仕様を理解し、どういうアーキテクチャで動くのかを理解する
	何を対応する必要があるか理解する

互いにコミュニケーションを取る必要がある

複数人のPJであるとコミュニケーション必要

そもそも障害を検知するしくみが　

nagios/App::MadEye/mon

OpsとDevで取り決めたフォーマットで作ることが重要

役立つログ
500 status, 404 statusをチェックしたほうが良い

accesslog
・時間単位でローテーション

applicatonlog
日単位でローテーション

error_log


mysql slow log
日単位でローテンションしてる

mysqlの slow log
役立つ、DBがボトルネックになることが多い

Komainuを作った
	forkモデル

gearman
cloudforcast

Cronx

deploy時間を記録するAgent

======================================================
闇のEメール伝説 [en] [any][library]
Ricardo Signes
@rjbs
13:40-14:20
======================================================
pobx.com

優先されてきたのは互換性。

みんなのコードが腐っているから


EMAIL::SIMPLE
シンプルと言いつつ、いろんな制約がある
Plain ASCII body
Not a reply 

EMAIL::MIME

EMAIL:MESSAGE

SPAMMERS
嫌われ者

RFC 724
	ヘッダの折りたたみ
	連続した空白・コメントを自由に挿入可

	デリミタ代わりのコメントは空白とみなす

	コメント、空白文字、開業の類

RFC2822

SMTP'S SHADOW
	文字数制限あり
	折りたたみやエンコーディングなし

	MIME


=======================================================
Evolution of API With Blogging [ja] [any][app]
Takatsugu Shigeta
@comewalk six apart
14:40-15:20
======================================================
History of Blogging
1994-2001
weblog 1994

blog 2000

MT 2001/10

2004 BLOG/HACKS


AtomPub
XML::Atom::Clinets;
XML::Atom::Entry;

WSSE

OpenID
Net::OpenID::Consumer

PubSubHubbub


explorer.metacpan.org

tools.ietf.org/html/rfc5789

http://camlistore.org/

======================================================
少人数でのWebアプリ開発 - CGIからPSGIまでの変遷 [ja] [beginner][app]
@aloelight
15:20-15:40
======================================================
Editor
	Padre
	Mi

YAPC AISIA 2007～2011
	CGI
	ModPerl
	PSGI

2006/10-2007/04
	CGI プログラマ
	scp deploy
	人力バージョニング

Excelでタスク管理
	更新されない
	更新したけど、共有されな

2007/04-2009/10
	RSSの利用で情報を集める
	YAPCに参加してModePerlに変更
	trac+svn

	svn checkoutでデータ移行

DevからDevOpsへ
	自分の為から、ログを出すように
	保守しやすいコード
	負荷が高い仕様を考えなおしてもらう

	開発サーバ上での直接作業による弊害
	複数人のファイルの奪い合い
	エラーがあると他の人がうごかせない
	テストがほとんどない

2009/10-
	PSGI期
	セットアップが簡単
	WAFを使いやすい

	Catalyst,Dancerなじみが無かった

	Plack+Moose

	CPAN形式のプロジェクト構成

	個人環境での開発

	テストの習慣化
	quickrun.vim

	Facebookで上司、社長、その他社内の偉い人と友人になる

2011年の開発スタイル
	PSGI/PlackベースWAF

	Jenkins,Ukigumo

	Curton
	pfperl

小規模だと変更も楽

=======================================================
あんなテスト、こんなテスト [ja] [any][testing]
tsucchi 凸版印刷
16:00-16:20
======================================================

テストのやりにくいテストのどうやるかの紹介。

warn/carpの出力を確認したい
IO::Scalar

Capture::Tyny

引数テスト
	Get::Option
	@ARGVを書き換える

時刻
	ログ日付フォーマット
	Test::MockTime
	Time::Mock

DB
	DBD::Mock
	ストアドプロシジャのテスト
	Test::Mysqld
	Test::Fixture::DBI

テスト中にexitが呼ばれると、意図せずテストが通る
	exitの上書き

	xUnit setup/tearDown
	Hook::LexWrap

Q&A
	tokuhiromさん？
	Test::Moreのバージョンをあげて下さい
		or
	no_planにしないで下さい

※
exiteの話は古いTest::Moreだとdone_testingが、
無いからっていうことなのかな？

===================================
PerlでJCL、基幹バッチをダウンサイジング [ja] [any][app]
minemaz
16:00-16:20
======================================================
※聞きトラブルで途中から聞けた

Parse::Eyapp
PDF::Haru

======================================================
Perlで仮想サーバ制御（ゆるひら） [HIRATA, Satoshi, ja] [intermediate][infra] 
@debility
fusic.co.jp
======================================================
Perlで仮想サーバを動かす話
VPS
AmazonEC2
開発環境として

PerlからlibVirtを触る

Sys::Virt

libvirtのバージョンでモジュールのバージョンも変わる

NET::AMQP
Carrot

Fusicという会社
	CakePHP Ruby on Rails

use Sys::Guestfs;
use Teng;

zenpre.net
	ustreamと同期できる

============================================================
LT Day 2 [ja] [any][other]
Daisuke Maki
============================================================
--------------------------------------
kiwanami
--------------------------------------
「Perl, Emacs and Async」

ぼくのかんがえたさいきょうのてきすとえでぃた
？？？


--------------------------------------
深町英太郎
--------------------------------------
「Perl5⇒ComonLisp⇒Perl5」

Common Lispに比べると、Perlは小さくて良い。

--------------------------------------
株式会社ガイアックス 鳥居晋太郎
@twodollers
--------------------------------------
「福岡の話」
perl暦12年
一緒に、事務所立ち上げやってくれる人募集

--------------------------------------
azuma kuniyuki
--------------------------------------
「bounce Hammer」

Server Engineer

bouncehammer.jp

--------------------------------------
株式会社ライブドア
@woremacx
--------------------------------------
ロケタッチの紹介

Mashup Awards7(#MA7)にもAPI使って参加してね。

FB上にフォーラムがあるので、質問してね

--------------------------------------
Yappo
--------------------------------------
ツールを作って、開発環境を整える話

gyazoサーバ？
sopstate

--------------------------------------
@tomiru Naoki Tomita
--------------------------------------
最近upされたおもしろいモジュール

CPANをチェックする人は暇な人である

AAAAAAAAA というモジュール
Mooseを高速化→Mouse→Moo→Mo→M(実装なし)
Acme::Teddy → 全熊に捧ぐ

--------------------------------------
@tokuhirom
--------------------------------------
File::Find;
File::FindRule;

上記は少し面倒。

File::Zglobを作った。

DBI::Inspector;

Daiku ←rake

App::watcher;
autobox::Encode;

cpan-outdated

Cache::KyotoTycoon ？？

--------------------------------------
ミクシィ
--------------------------------------
静的解析するプログラム

技術的負債の見える化

王様モジュール･･･多くの依存関係があるもの
最長不倒モジュール･･･沢山修正が加えられているもの


詳しくはWeb+DB 62

--------------------------------------
Kenichi Ishigaki
--------------------------------------
CPAN Author Top10?

acume.cpanauthors.org

--------------------------------------
kamipo
--------------------------------------

MessagePackの中身を見るもの？

--------------------------------------
yuusukebe
--------------------------------------
「ぼくのかんがえたさいきょうのえろさいとの舞台裏」

改良毎にアクセス数が増えている実績を紹介
北海道高校生akiyamaが登壇

--------------------------------------
TAKESAKO
--------------------------------------
Acme::MineChan

マインスイーパーを解く、モジュール。

※すごかった！

--------------------------------------
makamaka
--------------------------------------
Perlのカードゲームの抽選会

==========================================================
Managing A Band Of Hackers [ja] [any][community]
Hideo Kimura
@hideki DeNA
18:00-18:40
==========================================================
1990年生まれのage 41ｗ

経歴
	1996-2000
	ISP

2000-2007
	my own company

2007-2009
	Serbver hosting comapy

2009-
	DeNA

なぜマネージャーが必要か？
	1+1>=2 にするため

マネージャーの仕事
・project management
	プロダクトのライフサイクルを管理する

・personal matters
	人事
	その人が何をしたいか汲み取りアサイン
	評価

・その他
	事務
	稟議、出張準備
	会議が増える

マネージャーになるには、エンジア経験が必要。
Hackerは、飽きやすい、興味が優先、、寂しがりや、朝遅く夜も遅い、KY。

マネージャーが気をつけること
	delegation･･･任せること
	自分は10人のチームになったところで、コードを書くのを辞めた。
	丸投げと、任せるは異なる。失敗はマネージャーが負う。

bad new first
TMTOWTDIから、多様性の許容

Being Geekと言う、オライリーの本の紹介
マネージャーになるのに役立つ

マネージャーになる人は、優秀なエンジニアでなければ駄目だと思う。
キャリアとしてマネージャーへの道も考えに入れてみて欲しい


==========================================================
Closing [en] [any][community]
Daisuke Maki
18:40-19:00
==========================================================
ベストトーク賞の発表

3位 Webアプリでパスワード保護はどこまでやればいいか
guset speakerは対象にならないが、同率
	Perl 5.16 and beyond
	Carton: CPAN dependencies manager 
	闇のEメール伝説
2位 Perlで無理ゲーム攻略
1位 Perlで構築された中規模サイトのDC引っ越し記録

