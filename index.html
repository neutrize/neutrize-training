import { useState } from "react";

const STAFF = [
  { id:"akubo", name:"秋保まこ", role:"スタッフ", initial:"秋" },
  { id:"kasai", name:"笠井涼花", role:"スタッフ", initial:"笠" },
  { id:"okazaki", name:"岡崎颯太", role:"スタッフ", initial:"岡" },
];
const ADMINS = [
  { id:"ueda", name:"植田孝倫", role:"管理者", initial:"植", isAdmin:true, canEdit:true },
  { id:"oshima", name:"大島香純", role:"管理者", initial:"大", isAdmin:true, canEdit:true },
  { id:"ujihira", name:"氏平実里", role:"管理者", initial:"氏", isAdmin:true, canEdit:false },
  { id:"ishii", name:"石井渚", role:"管理者", initial:"石", isAdmin:true, canEdit:false },
  { id:"kondo", name:"近藤千寿", role:"管理者", initial:"近", isAdmin:true, canEdit:false },
];

const MENUS = [
  { id:"shampoo", label:"シャンプー", color:"#5B7A9E", sections:[
    { name:"準備", items:[
      {text:"施術前にシャンプー台・ボウルの清潔確認",req:true},
      {text:"タオルを適温に準備",req:false},
      {text:"お湯の温度確認（38℃前後）",req:true},
      {text:"お客様の首元・耳周りの保護",req:true},
      {text:"エプロン着用・手洗い完了",req:false},
      {text:"使用するシャンプー剤の確認・選定",req:false},
    ]},
    { name:"来店誘導・声かけ", items:[
      {text:"シャンプー台への誘導を穏やかに行う",req:true},
      {text:"倒れる際の声かけ（「ゆっくりどうぞ」）",req:true},
      {text:"首の高さ・角度の確認",req:true},
      {text:"温度確認の声かけ",req:true},
    ]},
    { name:"クレンジング", items:[
      {text:"頭皮全体への均一な塗布",req:true},
      {text:"生え際・もみあげ・うなじへの塗布もれなし",req:true},
      {text:"適切な放置時間の管理",req:true},
      {text:"乳化の実施",req:true},
      {text:"すすぎ30秒以上・残留なし確認",req:true},
    ]},
    { name:"シャンプー", items:[
      {text:"適量の泡立て",req:true},
      {text:"指の腹のみ使用（爪を立てない）",req:true},
      {text:"頭頂部・側頭部・後頭部・前頭部を漏れなく洗う",req:true},
      {text:"生え際・耳後ろ・うなじを丁寧に洗う",req:true},
      {text:"圧の強さをゲストの反応で調整",req:false},
      {text:"心地よいリズムのマッサージ",req:false},
    ]},
    { name:"すすぎ", items:[
      {text:"シャワーヘッドを頭皮に密着させて流す",req:true},
      {text:"頭皮→毛先の順で流す",req:true},
      {text:"顔・耳へのシャワー飛散に注意",req:true},
      {text:"すすぎ残しゼロの確認",req:true},
      {text:"水温を最後まで維持",req:false},
    ]},
    { name:"タオルドライ", items:[
      {text:"強く擦らず・押し当てて吸水",req:true},
      {text:"頭皮から毛先へ順に水分除去",req:false},
      {text:"耳の中・生え際の水分も取る",req:false},
    ]},
    { name:"仕上げ・接客", items:[
      {text:"起こす際の声かけ",req:true},
      {text:"タオルターバンの巻き方確認",req:false},
      {text:"「いかがでしたか？」の一声",req:false},
    ]},
  ]},
  { id:"dry", label:"ドライ・ブロー", color:"#8E7A5B", sections:[
    { name:"準備", items:[
      {text:"ブラシ・コームの清潔確認",req:true},
      {text:"ゲストの仕上げイメージの再確認",req:true},
    ]},
    { name:"タオルドライ", items:[
      {text:"押し当てて吸水（擦らない）",req:true},
      {text:"根元の水分を重点的に取る",req:true},
      {text:"毛先のもつれを無理に引っ張らない",req:true},
    ]},
    { name:"ラフドライ", items:[
      {text:"根元から乾かす順序を守る",req:true},
      {text:"ドライヤーの熱を一点集中させない",req:true},
      {text:"風の向きを根元→毛先に合わせる",req:true},
      {text:"頭皮・根元を8割以上乾かす",req:true},
    ]},
    { name:"ブロー仕上げ", items:[
      {text:"優しいタッチで丁寧に扱う",req:true},
      {text:"キューティクルを整える方向に風を当てる",req:true},
      {text:"熱と冷風の使い分け（熱→冷で形状固定）",req:true},
      {text:"顔周り・前髪の仕上げを最後に丁寧に行う",req:true},
    ]},
    { name:"仕上げ確認", items:[
      {text:"全体のシルエットバランス確認",req:true},
      {text:"艶・まとまりの確認",req:true},
      {text:"ゲストへ仕上がりの鏡確認",req:true},
    ]},
  ]},
  { id:"color", label:"カラー", color:"#7E6B8E", sections:[
    { name:"カウンセリング・診断", items:[
      {text:"希望カラーをヒアリング（画像・言葉）",req:true},
      {text:"ベースの明るさ（レベル）確認",req:true},
      {text:"ダメージ度・髪質の診断",req:true},
      {text:"矯正・パーマ履歴の確認",req:true},
      {text:"カラー履歴の確認",req:true},
      {text:"アレルギー・パッチテストの確認",req:true},
      {text:"施術内容・料金・所要時間の事前説明",req:true},
    ]},
    { name:"薬剤選定", items:[
      {text:"オキシ濃度の選定（3%/6%/9%）",req:true},
      {text:"色味・処方比率の決定",req:true},
    ]},
    { name:"塗布", items:[
      {text:"ブロッキングの正確さ",req:true},
      {text:"塗布量の均一さ",req:true},
      {text:"地肌への薬剤付着・刺激確認",req:true},
      {text:"毛先のオーバーラップに注意",req:true},
    ]},
    { name:"放置・管理", items:[
      {text:"放置時間をタイマーで管理",req:true},
      {text:"ゲストの状態（かゆみ・違和感）確認",req:true},
      {text:"テストストランドでの発色確認",req:true},
    ]},
    { name:"流し・仕上げ", items:[
      {text:"ぬるま湯での丁寧な流し",req:true},
      {text:"乳化をしっかり行う",req:true},
      {text:"仕上がりカラーのトーン・色味確認",req:true},
      {text:"ゲストへ仕上がり説明（色落ち変化も含む）",req:true},
    ]},
    { name:"カルテ記録", items:[
      {text:"使用薬剤名・オキシ濃度・ミックス比率の記録",req:true},
      {text:"放置時間の記録",req:true},
      {text:"仕上がりレベル・色味の記録",req:true},
    ]},
  ]},
  { id:"bleach", label:"ブリーチ", color:"#C4943A", sections:[
    { name:"カウンセリング・診断", items:[
      {text:"希望の明るさ・デザインのヒアリング",req:true},
      {text:"ダメージ度の詳細診断（0〜5段階）",req:true},
      {text:"過去のブリーチ・パーマ・縮毛矯正履歴の確認",req:true},
      {text:"毛髪強度・弾力の確認（引っ張りテスト）",req:true},
      {text:"施術リスクの説明と同意取得",req:true},
      {text:"料金・所要時間・複数回施術の可能性の説明",req:true},
    ]},
    { name:"塗布", items:[
      {text:"ブロッキングの正確さ・均等さ",req:true},
      {text:"根元→中間→毛先の塗布順序",req:true},
      {text:"塗布量の均一さ（ムラなし）",req:true},
      {text:"根元の体温部分は最後に塗布",req:true},
    ]},
    { name:"放置・リフトアップ管理", items:[
      {text:"放置時間のタイマー管理",req:true},
      {text:"15〜20分おきにリフト具合を確認",req:true},
      {text:"引っ張りテストで毛髪強度を随時確認",req:true},
      {text:"オーバープロセスの兆候を見逃さない",req:true},
      {text:"判断が難しい場合は即座に管理者へ報告",req:true},
    ]},
    { name:"流し・ケア・仕上げ", items:[
      {text:"ぬるま湯での速やかな流し",req:true},
      {text:"酸熱または集中ケアトリートメントの適用",req:true},
      {text:"ゲストへの仕上がり説明",req:true},
      {text:"自宅ケアアドバイス",req:true},
    ]},
  ]},
  { id:"counseling", label:"カウンセリング", color:"#6B8E6B", sections:[
    { name:"来店・導入", items:[
      {text:"笑顔・穏やかな声でお出迎え",req:true},
      {text:"ゲストの声のトーン・スピードに自分を合わせる",req:true},
      {text:"過去の来店履歴・カルテを事前に確認しておく",req:true},
    ]},
    { name:"ヒアリング", items:[
      {text:"「イメージはありますか？」で開始",req:true},
      {text:"ライフスタイル・職場・スタイリング時間を確認",req:true},
      {text:"今の髪の悩み・コンプレックスを丁寧に聴く",req:true},
    ]},
    { name:"診断・提案", items:[
      {text:"骨格・顔型・髪質・ダメージ度を診断",req:true},
      {text:"「なぜこの提案か」を根拠とともに言語化する",req:true},
      {text:"専門用語を使わず、伝わる言葉で話す",req:true},
    ]},
    { name:"施術内容の説明・合意", items:[
      {text:"使用薬剤の種類・選定理由を言葉で伝える",req:true},
      {text:"所要時間を具体的に伝える",req:true},
      {text:"料金を施術前に必ず確認・合意を得る",req:true},
      {text:"リスクがある場合は正直に説明し同意を取る",req:true},
    ]},
    { name:"ホームケア・次回提案", items:[
      {text:"今日の施術に合ったホームケアアドバイスを伝える",req:true},
      {text:"次回来店の目安タイミングを具体的に伝える",req:true},
    ]},
    { name:"カルテ記録", items:[
      {text:"要望・希望スタイルをカルテに記録",req:true},
      {text:"提案内容と合意事項を記録",req:true},
      {text:"次回提案・来店タイミングを記録",req:true},
    ]},
  ]},
  { id:"treatment", label:"トリートメント", color:"#5B8E7A", sections:[
    { name:"診断・選定", items:[
      {text:"髪質診断（硬さ・太さ・ダメージ度・水分量）",req:true},
      {text:"oggiotto 11種からの最適配合の決定",req:true},
      {text:"選定理由をゲストに言葉で説明",req:true},
    ]},
    { name:"塗布・浸透", items:[
      {text:"内側から外側・根元から毛先への塗布",req:true},
      {text:"毛先・ダメージ部位への重点塗布",req:true},
      {text:"放置時間のタイマー管理",req:true},
      {text:"「温度はいかがですか？」の確認",req:true},
    ]},
    { name:"流し・仕上げ", items:[
      {text:"ぬるま湯での丁寧な流し（すすぎ残しなし）",req:true},
      {text:"仕上がりの手触り・艶の確認",req:true},
      {text:"ゲストへ触感を確認してもらう",req:true},
    ]},
    { name:"カルテ記録", items:[
      {text:"使用したoggiotto品番・配合比率の記録",req:true},
      {text:"仕上がり手触り評価の記録",req:true},
    ]},
  ]},
  { id:"spa", label:"ヘッドスパ", color:"#5B8E8E", sections:[
    { name:"準備・空間設定", items:[
      {text:"個室の清潔・香り・照明・音楽の確認",req:true},
      {text:"ゲストへの事前説明（流れ・所要時間）",req:true},
    ]},
    { name:"頭皮診断", items:[
      {text:"頭皮の状態確認（乾燥・脂性・敏感・炎症なし）",req:true},
      {text:"頭皮の硬さ・血行状態の確認",req:true},
      {text:"診断内容をゲストに伝える",req:true},
    ]},
    { name:"マッサージ", items:[
      {text:"首・肩のほぐし（上から下へ）",req:true},
      {text:"側頭筋・後頭部のほぐし",req:true},
      {text:"圧の強さをゲストの反応で調整",req:true},
      {text:"「気持ちいいですか？」の確認",req:true},
    ]},
    { name:"仕上げ", items:[
      {text:"丁寧なすすぎ・後処理",req:true},
      {text:"起き上がる際のゆっくりした声かけ",req:true},
      {text:"次回スパのタイミング提案",req:false},
    ]},
  ]},
  { id:"straighten", label:"縮毛矯正", color:"#8B7355", sections:[
    { name:"カウンセリング・診断", items:[
      {text:"クセの強さ・種類の診断",req:true},
      {text:"ダメージ度の診断（0〜5段階）",req:true},
      {text:"過去の縮毛矯正・パーマ履歴の確認",req:true},
      {text:"施術リスクの説明と同意取得",req:true},
      {text:"料金・所要時間の事前説明",req:true},
    ]},
    { name:"1剤塗布・軟化", items:[
      {text:"ブロッキングの正確さ",req:true},
      {text:"均一塗布・ダメージ部位への過剰塗布を避ける",req:true},
      {text:"地肌への付着・刺激確認",req:true},
      {text:"テストストランドで軟化度確認",req:true},
      {text:"判断が難しい場合は管理者に報告",req:true},
    ]},
    { name:"流し・アイロン", items:[
      {text:"ぬるま湯での丁寧な流し",req:true},
      {text:"アイロン温度の設定（160〜180℃）",req:true},
      {text:"適切な角度でひきだす",req:true},
      {text:"根元〜毛先まで一方向にスライド",req:true},
      {text:"アイロン後の冷却確認",req:true},
    ]},
    { name:"2剤・仕上げ", items:[
      {text:"2剤の適量・均一塗布",req:true},
      {text:"放置時間のタイマー管理",req:true},
      {text:"2剤の完全流し",req:true},
      {text:"ブロー仕上げ・鏡確認",req:true},
    ]},
    { name:"カルテ記録", items:[
      {text:"使用薬剤・濃度・放置時間の記録",req:true},
      {text:"アイロン温度の記録",req:true},
    ]},
  ]},
  { id:"cut", label:"カット", color:"#6B7A8E", sections:[
    { name:"カウンセリング", items:[
      {text:"希望スタイルのヒアリング（画像・言葉）",req:true},
      {text:"骨格・顔型・首の長さの確認",req:true},
      {text:"ライフスタイル・スタイリング時間の確認",req:true},
      {text:"料金・所要時間の事前説明",req:true},
    ]},
    { name:"カット施術", items:[
      {text:"ブロッキングの正確さ・均等さ",req:true},
      {text:"ガイドに沿った正確なカット",req:true},
      {text:"左右対称の確認（都度チェック）",req:true},
      {text:"顔周り・もみあげの自然なつながり",req:true},
      {text:"えり足・うなじラインの整え",req:true},
    ]},
    { name:"仕上げ確認", items:[
      {text:"乾いた状態でのシルエット全体確認",req:true},
      {text:"ゲストに鏡で確認（正面・バックミラー）",req:true},
      {text:"仕上がりの意図を言葉で説明",req:true},
    ]},
  ]},
  { id:"set", label:"セット・アレンジ", color:"#7A6B8E", sections:[
    { name:"カウンセリング", items:[
      {text:"希望スタイル・仕上げイメージのヒアリング",req:true},
      {text:"使用シーン（結婚式・成人式・普段使い等）の確認",req:true},
      {text:"所要時間・料金の事前説明",req:true},
    ]},
    { name:"セット・アレンジ施術", items:[
      {text:"コテ・アイロンの温度設定（髪質に合わせて）",req:true},
      {text:"左右のバランス確認（都度チェック）",req:true},
      {text:"ゴムやピンが見えていないか確認",req:true},
      {text:"顔周り・前髪の仕上げを丁寧に行う",req:true},
    ]},
    { name:"仕上げ・固定", items:[
      {text:"スプレーでの仕上げ固定（適量・均一）",req:true},
      {text:"全方向からのシルエット確認",req:true},
      {text:"ゲストへ鏡確認",req:true},
      {text:"セット後の直し方アドバイス",req:true},
    ]},
  ]},
  { id:"perm", label:"パーマ", color:"#8E6B7A", sections:[
    { name:"カウンセリング・診断", items:[
      {text:"希望カール・ウェーブのヒアリング",req:true},
      {text:"ダメージ度・髪質の診断",req:true},
      {text:"パーマ・縮毛矯正の履歴確認",req:true},
      {text:"施術リスクの説明と同意取得",req:true},
      {text:"料金・所要時間の事前説明",req:true},
    ]},
    { name:"ロッドワインディング", items:[
      {text:"ブロッキングの正確さ・均等さ",req:true},
      {text:"巻きつけテンションの均一さ",req:true},
      {text:"巻き方向の一貫性",req:true},
      {text:"全体のロッド配置バランス確認",req:true},
    ]},
    { name:"1剤塗布・軟化", items:[
      {text:"均一な薬剤塗布",req:true},
      {text:"1剤塗布後 たれていないか確認",req:true},
      {text:"テストカールで軟化度確認",req:true},
      {text:"判断が難しい場合は管理者に報告",req:true},
    ]},
    { name:"流し・2剤・仕上げ", items:[
      {text:"中間流しの丁寧さ",req:true},
      {text:"2剤の均一塗布・放置時間管理",req:true},
      {text:"巻き残しがないか確認",req:true},
      {text:"スタイリング方法の説明",req:true},
      {text:"ゲストへ仕上がり確認・ホームケアアドバイス",req:true},
    ]},
  ]},
  { id:"oggiotto", label:"oggiotto知識", color:"#9A6B4B", sections:[
    { name:"SALON CARE 製品知識", items:[
      {text:"RL（リセットローション）：マイナスイオンで残留物を除去するクレンジング処理剤",req:true},
      {text:"PU（ペネトレーションウーレ）：尿素で髪をゆるめ栄養の通り道を整える浸透促進剤",req:true},
      {text:"BC（ブラッディーコンプレックス）：低・中・高分子ケラチンをバランスよく配合した強化型ケラチン複合体",req:true},
      {text:"BM（ブラッディーモイスチャー）：加水分解コラーゲン・ヒアルロン酸配合の保水型コラーゲン",req:true},
      {text:"HP（ハイドロップポリフェ）：余分な水分を除去しタンパク質を引き締める疎水型ポリフェノール",req:true},
      {text:"CH（クロスリンクヘマ）：システイン結合を形成しパーマ持続・カラー発色を促進する架橋型ヘマチン",req:true},
      {text:"AA（アーマーキューティクルアシッド）：擬似キューティクルを形成しpHコントロールで保護する保護型キトサン",req:true},
      {text:"VCM（ベゼル CMCミスト）：水分・油分・薬剤を運ぶ通り道をつくる補修型CMC（マルチアイテム）",req:true},
      {text:"BCC（ボーン CMCクリーム）：脂質を補給し毛髪内部の骨格を強化する接着型CMC",req:true},
      {text:"MCM（マスクル CMCミルキ）：擬似コルテックスをつくる補修型CMC（マルチアイテム）",req:true},
      {text:"SCO（スキン CMCオイル）：毛髪表面に油分・ツヤを与えキューティクルを保護する補修型CMC",req:true},
      {text:"SA（ストレートアシッド）：コルテックス間の結合のゆがみをととのえクセを緩和する酸熱型ケラチン複合体",req:true},
      {text:"CM（コネクトマキシム）：保湿力・弾力・柔軟性を高める純度100%コラーゲンPPTパウダー（熱ダメージ予防）",req:true},
    ]},
    { name:"AROMA CARE 知識", items:[
      {text:"ケモタイプ精油を使用・基材に対する推奨濃度1%",req:true},
      {text:"shine（シャイン）活性：集中力・記憶力を高める朝向けブレンド",req:true},
      {text:"beauty（ビューティー）活性：お肌・身体のメンテナンスを行う美容ブレンド",req:true},
      {text:"refresh（リフレッシュ）活性：気持ちをリセットし呼吸を整える",req:true},
      {text:"grow（グロウ）活性：沈んだ心を癒して高め血行を促進するエイジングケアブレンド",req:true},
      {text:"scalp（スキャルプ）活性：脳のよどみを晴らし肌トラブルを改善する頭皮ケアブレンド",req:true},
      {text:"cool（クール）鎮静：クールダウンさせ疲れやモヤモヤを解消するミントブレンド",req:true},
      {text:"care（ケア）鎮静：慢性的な疲れを解消し血行を促進するデトックスブレンド",req:true},
      {text:"relax（リラックス）鎮静：リラックスさせストレス・疲労を軽減する柑橘系の甘い香り",req:true},
      {text:"moon（ムーン）鎮静：眠りの質を改善し緊張をほぐすおやすみブレンド",req:true},
    ]},
    { name:"使用シーン・組み合わせ", items:[
      {text:"RL・PUは前処理で使用し、その後BC・BM等でケアする流れを理解している",req:true},
      {text:"CHはカラー乳化に適しており、パーマ・カラーの両施術で活用できる",req:true},
      {text:"HP・AAは後処理・仕上げに使用し施術の持続性を高めることを理解している",req:true},
      {text:"VCM・MCM・SCOはインバス・アウトバス両方で使用可能なマルチアイテム",req:true},
      {text:"アロマは活性5種・鎮静4種の計9種を効果・香りに合わせてゲストに提案できる",req:true},
    ]},
  ]},
];

const CHAPTERS = [
  {no:1,title:"NEUTRIZEとはどんな場所か",sub:"理念・名前・ブランドの根っこを理解する",body:"「NEUTRIZE」はNeutral＋izeから生まれた造語。余計なものを足すのではなく、余分なものをそぎ落とす。2010年創業、2012年法人化。HPBアワード5年連続受賞（2024〜26年SILVER AWARD）。口コミ評価4.95。oggiotto全国上位1%正規取扱店。"},
  {no:2,title:"ゲストが選ぶ理由",sub:"NEUTRIZEの強みを自分の言葉にする",body:"①設計力——骨格・髪質だけでなくライフスタイル・今の気分まで読んで設計する。②通うほどに変わる——来るたびに髪の状態と扱いやすさが積み上がる設計。③説明できる誠実さ——薬剤の選定理由・変化を言葉にして伝える。"},
  {no:3,title:"NEUTRIZEで働くということ",sub:"5つの価値観を自分の中に根づかせる",body:"①無理のない自分でいること ②リセットと成長を繰り返せる環境 ③整えることを届け、自分も整えられる ④トレンドを流されずに活かす感性 ⑤NEUTRIZEの空気感に寄せていく努力"},
  {no:4,title:"主力メニューを知る",sub:"「なぜそれか」を語れることが差別化になる",body:"髪質改善・透明感カラー・高濃度水素カラー・oggiotto・似合わせカット・個室ヘッドスパ——すべてのメニューに「なぜこの人にこれを提案するか」の根拠を持つ。"},
  {no:5,title:"美容師に必要な10の要素",sub:"カウンセリング5つ×施術5つ",body:"①導入 ②洞察 ③受容 ④計画 ⑤提案 ／ ⑥感知 ⑦説明 ⑧技術 ⑨管理 ⑩発信——すべての要素に「なぜ」を持つことがNEUTRIZEのスタイリストの証。"},
  {no:6,title:"接客の基本マナーと身だしなみ",sub:"NEUTRIZEの空気感を体現する",body:"服装・髪型・香り・表情・声のトーン——自分がNEUTRIZEの作品である意識を持つ。NGな言動：逆説フレーズ（「でも〜」）・専門用語の多用・私的スマホ操作。"},
  {no:7,title:"カウンセリングの技術",sub:"ゲストの「今日」を読む力",body:"価格重視型・クオリティ重視型・接客重視型・雰囲気重視型——ゲストタイプを見極め、コンプレックスをメリットに変換する。「綺麗になった」より「自分のことをわかってくれた」と感じてもらう。"},
  {no:8,title:"施術中・お見送り・フォロー",sub:"最後まで途切れない体験をつくる",body:"沈黙を怖がらない。お見送りはゲストの最後の記憶——次回来店タイミング・ホームケアアドバイスを添えて。HPB・SNS・DMでサロン外の接点を途切れさせない。"},
  {no:9,title:"カルテと情報管理",sub:"ゲストとの「約束」を記録する",body:"①施術内容 ②使用薬剤（濃度・放置時間・比率） ③髪の状態 ④要望・好み・口癖 ⑤次回への提案——担当が変わっても「ちゃんと覚えていてくれている」がリピートの理由になる。"},
  {no:10,title:"クレーム対応と問題解決",sub:"成長の機会として向き合う",body:"①最後まで聴く ②共感を示す ③事実確認 ④上司に報告 ⑤解決策提示 ⑥再発防止の言語化。言い訳・自分で抱え込む・感情的になる——これらは信頼を一瞬で失う。"},
  {no:11,title:"成長マインドとキャリアビジョン",sub:"NEUTRIZEとともに育つ",body:"前半1〜6ヶ月：施術フロー・接客マナー・カルテ記録を習慣化。後半7〜12ヶ月：担当ゲストを持ち10の要素を意識した施術へ。2年目以降：独自スタイル確立・専門技術で差別化・後輩育成。"},
  {no:12,title:"oggiotto製品知識",sub:"SALON CARE / AROMA CARE を使いこなす",body:"【SALON CARE 13製品】RL→PU→BC/BM→HP/CH/AA→VCM/MCM/SCO→SA→CM の流れで理解する。\n\n【AROMA CARE 9種】活性ブレンド5種（shine・beauty・refresh・grow・scalp）＋鎮静ブレンド4種（cool・care・relax・moon）。ケモタイプ精油・基材推奨濃度1%。\n\n使い分けの基本：RL・PUで前処理 → BC・BMで補給 → HP・AA・CHで定着・後処理。VCM・MCM・SCOはインバス・アウトバス両対応のマルチアイテム。"},
];

const pal = { bg:"#f5f3ef", card:"#ffffff", border:"#e0dbd0", gold:"#b8960a", text:"#1a1a1a", muted:"#888880", accent:"#3a3a3a" };
const st = {
  app: { minHeight:"100vh", background:pal.bg, color:pal.text, fontFamily:"Georgia,'Times New Roman',serif", fontSize:15 },
  hdr: { background:"#1a1a1a", borderBottom:"1px solid #333", padding:"16px 20px", display:"flex", alignItems:"center", justifyContent:"space-between" },
  logo: { fontSize:14, fontWeight:400, letterSpacing:"0.3em", color:"#d4a800" },
  nav: { display:"flex", background:"#ffffff", borderBottom:`1px solid ${pal.border}` },
  nb: (a) => ({ flex:1, padding:"13px 0", fontSize:12, color:a?pal.gold:pal.muted, background:"none", border:"none", borderBottom:a?`2px solid ${pal.gold}`:"2px solid transparent", cursor:"pointer", letterSpacing:"0.1em" }),
  card: { background:pal.card, border:`1px solid ${pal.border}`, borderRadius:2, padding:"14px 16px", marginBottom:8, boxShadow:"0 1px 3px rgba(0,0,0,0.04)" },
  btn: (v) => ({ padding:v==="sm"?"5px 14px":"12px 24px", fontSize:v==="sm"?11:13, background:v==="p"?"#1a1a1a":"transparent", color:v==="p"?"#d4a800":pal.muted, border:`1px solid ${v==="p"?"#1a1a1a":pal.border}`, borderRadius:2, cursor:"pointer", letterSpacing:"0.08em" }),
  label: { fontSize:10, letterSpacing:"0.18em", color:pal.muted, marginBottom:14, textTransform:"uppercase" },
};

const makeEmpty = (menu) => {
  const o = {};
  menu.sections.forEach(sec => sec.items.forEach((_, i) => {
    o[`${sec.name}-${i}`] = { checked:false, evaluator:null, date:null };
  }));
  return o;
};
const makeReq = (menu) => {
  const o = {};
  menu.sections.forEach(sec => sec.items.forEach((item, i) => { o[`${sec.name}-${i}`] = item.req; }));
  return o;
};
const countDone = (checks) => Object.values(checks).filter(v => v && v.checked === true).length;
const isPassed = (menu, checks, req) => menu.sections.every(sec => sec.items.every((_, i) => {
  const k = `${sec.name}-${i}`;
  return !req[k] || (checks[k] && checks[k].checked === true);
}));

function Avatar({ s, size=34 }) {
  return <div style={{ width:size, height:size, borderRadius:"50%", background:"#e8e4dc", border:`1px solid ${pal.gold}66`, display:"flex", alignItems:"center", justifyContent:"center", fontSize:size*0.36, color:pal.gold, flexShrink:0 }}>{s.initial}</div>;
}
function Badge({ small }) {
  return <div style={{ display:"inline-flex", alignItems:"center", gap:4, background:"#f0f8ec", border:"1px solid #6aaa4a", borderRadius:2, padding:small?"2px 8px":"4px 12px", fontSize:small?10:12, color:"#3a7a20" }}>✓ 合格</div>;
}

function Login({ onLogin }) {
  const [mode, setMode] = useState(null);
  const [sel, setSel] = useState(null);
  const list = mode === "admin" ? ADMINS : STAFF;
  return (
    <div style={{ ...st.app, display:"flex", flexDirection:"column", alignItems:"center", justifyContent:"center", minHeight:"100vh", padding:24 }}>
      <div style={{ marginBottom:40, textAlign:"center" }}>
        <div style={{ fontSize:22, letterSpacing:"0.35em", marginBottom:8 }}>NEUTRIZE</div>
        <div style={{ fontSize:10, letterSpacing:"0.22em", color:pal.muted }}>STAFF TRAINING PORTAL</div>
      </div>
      {!mode && <div style={{ width:"100%", maxWidth:300 }}>
        <div style={{ ...st.label, textAlign:"center" }}>ログイン区分を選択</div>
        <button onClick={() => setMode("admin")} style={{ ...st.btn("p"), width:"100%", padding:"14px 0", marginBottom:10 }}>管理者</button>
        <button onClick={() => setMode("staff")} style={{ ...st.btn(), width:"100%", padding:"14px 0", color:pal.text }}>スタッフ</button>
      </div>}
      {mode && <div style={{ width:"100%", maxWidth:300 }}>
        <div style={{ ...st.label, textAlign:"center" }}>{mode === "admin" ? "管理者" : "スタッフ"}を選択</div>
        {list.map(a => (
          <div key={a.id} onClick={() => setSel(a)} style={{ ...st.card, display:"flex", alignItems:"center", gap:12, cursor:"pointer", border:`1px solid ${sel?.id===a.id?pal.gold:pal.border}`, marginBottom:8 }}>
            <Avatar s={a} /><div><div>{a.name}</div><div style={{ fontSize:11, color:pal.muted }}>{a.role}</div></div>
          </div>
        ))}
        {sel && <button onClick={() => onLogin(sel)} style={{ ...st.btn("p"), width:"100%", padding:"14px 0", marginTop:4, marginBottom:10 }}>ログイン</button>}
        <button onClick={() => { setMode(null); setSel(null); }} style={{ ...st.btn("sm"), color:pal.muted }}>← 戻る</button>
      </div>}
    </div>
  );
}

function ItemEditor({ menu, onClose, onSave }) {
  const [secs, setSecs] = useState(JSON.parse(JSON.stringify(menu.sections)));
  const [newT, setNewT] = useState({});
  const del = (si, ii) => setSecs(p => p.map((s, i) => i !== si ? s : { ...s, items: s.items.filter((_, j) => j !== ii) }));
  const add = (si) => {
    const t = (newT[si]||"").trim();
    if (!t) return;
    setSecs(p => p.map((s, i) => i !== si ? s : { ...s, items: [...s.items, { text:t, req:false }] }));
    setNewT(p => ({ ...p, [si]:"" }));
  };
  return (
    <div style={{ position:"fixed", inset:0, background:"rgba(0,0,0,0.5)", zIndex:100, overflowY:"auto", padding:16 }}>
      <div style={{ background:pal.card, borderRadius:4, maxWidth:560, margin:"0 auto", padding:20 }}>
        <div style={{ display:"flex", justifyContent:"space-between", alignItems:"center", marginBottom:16 }}>
          <div style={{ fontSize:14 }}>{menu.label} — 項目編集</div>
          <button onClick={onClose} style={{ ...st.btn("sm"), color:pal.muted }}>閉じる</button>
        </div>
        {secs.map((sec, si) => (
          <div key={si} style={{ marginBottom:16 }}>
            <div style={{ fontSize:11, color:pal.gold, marginBottom:8 }}>{sec.name}</div>
            {sec.items.map((item, ii) => (
              <div key={ii} style={{ display:"flex", alignItems:"center", gap:8, marginBottom:6 }}>
                <div style={{ flex:1, fontSize:13 }}>{item.text}</div>
                <button onClick={() => del(si, ii)} style={{ ...st.btn("sm"), color:"#c44", border:"1px solid #c44", padding:"3px 10px", fontSize:11 }}>削除</button>
              </div>
            ))}
            <div style={{ display:"flex", gap:8, marginTop:8 }}>
              <input value={newT[si]||""} onChange={e => setNewT(p => ({ ...p, [si]:e.target.value }))} onKeyDown={e => e.key==="Enter" && add(si)} placeholder="新しい項目を入力..." style={{ flex:1, background:pal.bg, border:`1px solid ${pal.border}`, borderRadius:2, padding:"6px 10px", fontSize:12, color:pal.text, fontFamily:"Georgia,serif" }} />
              <button onClick={() => add(si)} style={{ ...st.btn("sm"), color:pal.gold, border:`1px solid ${pal.gold}` }}>追加</button>
            </div>
          </div>
        ))}
        <button onClick={() => onSave(secs)} style={{ ...st.btn("p"), width:"100%", marginTop:8, padding:"12px 0" }}>保存する</button>
      </div>
    </div>
  );
}

function Checklist({ menu, existing, staffId, menuId, onSave, isAdmin, canEdit, readOnly, evaluator, req, onReq, onUpdateMenu, onBack }) {
  const [checks, setChecks] = useState(() => {
    const base = makeEmpty(menu);
    if (!existing.checks) return base;
    Object.keys(base).forEach(k => {
      const v = existing.checks[k];
      if (v && typeof v === "object" && "checked" in v) base[k] = v;
    });
    return base;
  });
  const [comment, setComment] = useState(existing.comment||"");
  const [saved, setSaved] = useState(false);
  const [editReq, setEditReq] = useState(false);
  const [showEditor, setShowEditor] = useState(false);

  const done = countDone(checks);
  const max = menu.sections.reduce((a, s) => a + s.items.length, 0);
  const pct = Math.round((done/max)*100);
  const passed = isPassed(menu, checks, req);
  const rTotal = Object.values(req).filter(Boolean).length;
  const rDone = menu.sections.reduce((a, sec) => a + sec.items.filter((_, i) => req[`${sec.name}-${i}`] && checks[`${sec.name}-${i}`]?.checked === true).length, 0);

  const toggle = (k) => {
    if (!isAdmin || readOnly) return;
    setChecks(p => {
      const cur = p[k];
      if (cur && cur.checked) return { ...p, [k]:{ checked:false, evaluator:null, date:null } };
      return { ...p, [k]:{ checked:true, evaluator, date:new Date().toLocaleDateString("ja-JP") } };
    });
  };
  const save = () => {
    onSave(staffId, menuId, { checks, comment, date:new Date().toLocaleDateString("ja-JP"), evaluator:isAdmin?evaluator:null, passed });
    setSaved(true); setTimeout(() => setSaved(false), 1500);
  };

  return (
    <div style={st.app}>
      {showEditor && <ItemEditor menu={menu} onClose={() => setShowEditor(false)} onSave={(s) => { onUpdateMenu(menuId, s); setShowEditor(false); }} />}
      <div style={st.hdr}>
        <button onClick={onBack} style={{ ...st.btn("sm"), color:"#aaa", border:"1px solid #444" }}>← 戻る</button>
        <div style={{ display:"flex", alignItems:"center", gap:8 }}>
          {canEdit && <button onClick={() => setShowEditor(true)} style={{ ...st.btn("sm"), color:pal.gold, border:`1px solid ${pal.gold}`, fontSize:11 }}>＋ 項目編集</button>}
          <div style={{ fontSize:12, color:"#aaa" }}>{menu.label}</div>
        </div>
      </div>
      <div style={{ padding:14 }}>
        <div style={{ ...st.card, marginBottom:14 }}>
          <div style={{ display:"flex", alignItems:"center", gap:16, marginBottom:10 }}>
            <div style={{ textAlign:"center", minWidth:52 }}>
              <div style={{ fontSize:26, color:menu.color }}>{pct}<span style={{ fontSize:13 }}>%</span></div>
              <div style={{ fontSize:10, color:pal.muted }}>{done}/{max}</div>
            </div>
            <div style={{ flex:1 }}>
              <div style={{ height:4, background:pal.border, borderRadius:2, overflow:"hidden", marginBottom:6 }}>
                <div style={{ height:"100%", width:`${pct}%`, background:menu.color, borderRadius:2, transition:"width 0.3s" }} />
              </div>
              <div style={{ fontSize:11, color:pal.muted }}>{menu.label} / {max}項目</div>
            </div>
            {passed && done > 0 && <Badge />}
          </div>
          <div style={{ borderTop:`1px solid ${pal.border}`, paddingTop:8, display:"flex", justifyContent:"space-between" }}>
            <div style={{ fontSize:11, color:pal.muted }}>必須項目 {rDone}/{rTotal}</div>
            {existing.evaluator && <div style={{ fontSize:11, color:pal.gold }}>最終評価: {existing.evaluator}　{existing.date}</div>}
          </div>
        </div>
        {isAdmin && !readOnly && (
          <div style={{ display:"flex", justifyContent:"flex-end", marginBottom:12 }}>
            <button onClick={() => setEditReq(p => !p)} style={{ ...st.btn("sm"), color:editReq?pal.gold:pal.muted, border:`1px solid ${editReq?pal.gold:pal.border}` }}>
              {editReq ? "★ 必須設定中" : "☆ 必須項目を編集"}
            </button>
          </div>
        )}
        {menu.sections.map(sec => (
          <div key={sec.name} style={{ marginBottom:14 }}>
            <div style={{ display:"flex", alignItems:"center", gap:7, marginBottom:8 }}>
              <div style={{ width:7, height:7, borderRadius:"50%", background:menu.color }} />
              <div style={{ fontSize:11, color:pal.accent, letterSpacing:"0.1em" }}>{sec.name}</div>
            </div>
            {sec.items.map((item, i) => {
              const k = `${sec.name}-${i}`;
              const v = checks[k];
              const checked = v && v.checked === true;
              const r = req[k];
              return (
                <div key={k} style={{ padding:"8px 12px", background:checked?menu.color+"14":pal.card, border:`1px solid ${checked?menu.color+"55":pal.border}`, borderRadius:2, marginBottom:5 }}>
                  <div style={{ display:"flex", alignItems:"flex-start", gap:8 }}>
                    {editReq
                      ? <div onClick={() => onReq(menuId, k, !r)} style={{ fontSize:14, color:r?pal.gold:"#ccc", cursor:"pointer", flexShrink:0, marginTop:1 }}>{r?"★":"☆"}</div>
                      : <div style={{ fontSize:12, color:r?pal.gold:"transparent", flexShrink:0, marginTop:2 }}>★</div>
                    }
                    <div onClick={() => toggle(k)} style={{ width:16, height:16, minWidth:16, borderRadius:2, border:`1.5px solid ${checked?menu.color:pal.border}`, background:checked?menu.color:"transparent", display:"flex", alignItems:"center", justifyContent:"center", marginTop:2, cursor:(isAdmin&&!readOnly)?"pointer":"default", flexShrink:0 }}>
                      {checked && <div style={{ color:"#fff", fontSize:10 }}>✓</div>}
                    </div>
                    <div style={{ flex:1 }}>
                      <div style={{ fontSize:13, color:checked?pal.text:pal.muted, lineHeight:1.5 }}>{item.text}</div>
                      {checked && v?.evaluator && <div style={{ fontSize:10, color:pal.gold, marginTop:3 }}>{v.evaluator}　{v.date}</div>}
                    </div>
                  </div>
                </div>
              );
            })}
          </div>
        ))}
        {isAdmin && !readOnly && <>
          <div style={{ marginTop:12 }}>
            <div style={{ fontSize:11, color:pal.muted, marginBottom:6 }}>評価コメント</div>
            <textarea value={comment} onChange={e => setComment(e.target.value)} placeholder="評価コメントを入力..." style={{ width:"100%", minHeight:68, background:pal.bg, border:`1px solid ${pal.border}`, borderRadius:2, padding:"9px 12px", color:pal.text, fontSize:13, resize:"vertical", boxSizing:"border-box", fontFamily:"Georgia,serif", lineHeight:1.6 }} />
          </div>
          <button onClick={save} style={{ ...st.btn("p"), width:"100%", marginTop:10, padding:"13px 0" }}>{saved?"保存しました":"保存する"}</button>
        </>}
        {readOnly && existing.comment && (
          <div style={{ ...st.card, marginTop:12 }}>
            <div style={{ fontSize:10, color:pal.muted, marginBottom:6 }}>評価コメント</div>
            <div style={{ fontSize:13, color:pal.text, lineHeight:1.7 }}>{existing.comment}</div>
          </div>
        )}
      </div>
    </div>
  );
}

function MenuList({ user, scores, onSave, isAdmin, canEdit, readOnly, menus, reqs, onReq, onUpdateMenu }) {
  const [sel, setSel] = useState(null);
  const sid = user.id;
  const sc = scores[sid]||{};
  if (sel) {
    const menu = menus.find(m => m.id === sel);
    return <Checklist menu={menu} existing={sc[sel]||{}} staffId={sid} menuId={sel} onSave={onSave} isAdmin={isAdmin} canEdit={canEdit} readOnly={readOnly} evaluator={user.name} req={reqs[sel]||makeReq(menu)} onReq={onReq} onUpdateMenu={onUpdateMenu} onBack={() => setSel(null)} />;
  }
  return (
    <div style={{ padding:16 }}>
      <div style={st.label}>メニュー別チェックリスト</div>
      {menus.map(m => {
        const msc = sc[m.id]||{};
        const checks = msc.checks && Object.keys(msc.checks).length > 0 ? msc.checks : makeEmpty(m);
        const done = countDone(checks);
        const max = m.sections.reduce((a, s) => a + s.items.length, 0);
        const pct = Math.round((done/max)*100);
        const passed = msc.passed || isPassed(m, checks, reqs[m.id]||makeReq(m));
        return (
          <div key={m.id} onClick={() => setSel(m.id)} style={{ ...st.card, cursor:"pointer" }}>
            <div style={{ display:"flex", justifyContent:"space-between", alignItems:"center", marginBottom:6 }}>
              <div style={{ display:"flex", alignItems:"center", gap:8 }}>
                <div style={{ width:7, height:7, borderRadius:"50%", background:m.color }} />
                <div style={{ fontSize:14 }}>{m.label}</div>
              </div>
              <div style={{ display:"flex", alignItems:"center", gap:8 }}>
                {passed && done > 0 && <Badge small />}
                <div style={{ fontSize:13, color:m.color }}>{pct}%</div>
              </div>
            </div>
            <div style={{ height:3, background:pal.border, borderRadius:2, overflow:"hidden", marginBottom:6 }}>
              <div style={{ height:"100%", width:`${pct}%`, background:m.color, borderRadius:2 }} />
            </div>
            <div style={{ display:"flex", justifyContent:"space-between" }}>
              <div style={{ fontSize:11, color:pal.muted }}>{done}/{max}項目</div>
              {msc.evaluator ? <div style={{ fontSize:11, color:pal.gold }}>評価: {msc.evaluator}　{msc.date}</div> : !readOnly ? <div style={{ fontSize:11, color:"#ccc" }}>未評価</div> : null}
            </div>
          </div>
        );
      })}
    </div>
  );
}

function Dashboard({ scores, menus, reqs, onSelect }) {
  const tMax = menus.reduce((a, m) => a + m.sections.reduce((b, s) => b + s.items.length, 0), 0);
  return (
    <div style={{ padding:"20px 16px" }}>
      <div style={st.label}>スタッフ進捗一覧</div>
      {STAFF.map(s => {
        const sc = scores[s.id]||{};
        const tDone = menus.reduce((a, m) => a + countDone(sc[m.id]?.checks||makeEmpty(m)), 0);
        const pct = Math.round((tDone/tMax)*100);
        const pass = menus.filter(m => tDone > 0 && (sc[m.id]?.passed || isPassed(m, sc[m.id]?.checks||makeEmpty(m), reqs[m.id]||makeReq(m)))).length;
        const evs = [...new Set(menus.map(m => sc[m.id]?.evaluator).filter(Boolean))];
        return (
          <div key={s.id} onClick={() => onSelect(s)} style={{ ...st.card, display:"flex", alignItems:"center", gap:12, cursor:"pointer" }}>
            <Avatar s={s} />
            <div style={{ flex:1 }}>
              <div style={{ display:"flex", justifyContent:"space-between", alignItems:"center", marginBottom:6 }}>
                <div style={{ fontSize:14 }}>{s.name}</div>
                <div style={{ display:"flex", alignItems:"center", gap:8 }}>
                  {pass > 0 && <div style={{ fontSize:11, color:"#3a7a20", background:"#f0f8ec", border:"1px solid #6aaa4a", borderRadius:2, padding:"1px 8px" }}>合格 {pass}/{menus.length}</div>}
                  <div style={{ fontSize:13, color:pal.gold }}>{pct}%</div>
                </div>
              </div>
              <div style={{ height:3, background:pal.border, borderRadius:2, overflow:"hidden", marginBottom:5 }}>
                <div style={{ height:"100%", width:`${pct}%`, background:pal.gold, borderRadius:2 }} />
              </div>
              {evs.length > 0 && <div style={{ fontSize:11, color:pal.muted }}>評価: {evs.join("・")}</div>}
            </div>
          </div>
        );
      })}
    </div>
  );
}

function StaffDetail({ staff, user, scores, onSave, menus, reqs, onReq, onUpdateMenu, onBack }) {
  const [sel, setSel] = useState(null);
  const sc = scores[staff.id]||{};
  const tMax = menus.reduce((a, m) => a + m.sections.reduce((b, s) => b + s.items.length, 0), 0);
  const tDone = menus.reduce((a, m) => a + countDone(sc[m.id]?.checks||makeEmpty(m)), 0);
  if (sel) {
    const menu = menus.find(m => m.id === sel);
    return <Checklist menu={menu} existing={sc[sel]||{}} staffId={staff.id} menuId={sel} onSave={onSave} isAdmin={true} canEdit={user.canEdit} evaluator={user.name} req={reqs[sel]||makeReq(menu)} onReq={onReq} onUpdateMenu={onUpdateMenu} onBack={() => setSel(null)} />;
  }
  return (
    <div>
      <div style={{ padding:"12px 16px", borderBottom:`1px solid ${pal.border}`, display:"flex", alignItems:"center", gap:10 }}>
        <button onClick={onBack} style={{ ...st.btn("sm"), color:pal.muted }}>← 戻る</button>
        <Avatar s={staff} size={26} />
        <div style={{ fontSize:14 }}>{staff.name}</div>
        <div style={{ marginLeft:"auto", fontSize:12, color:pal.gold }}>{Math.round((tDone/tMax)*100)}%</div>
      </div>
      <div style={{ padding:16 }}>
        <div style={st.label}>メニュー別評価</div>
        {menus.map(m => {
          const msc = sc[m.id]||{};
          const checks = msc.checks && Object.keys(msc.checks).length > 0 ? msc.checks : makeEmpty(m);
          const done = countDone(checks);
          const max = m.sections.reduce((a, s) => a + s.items.length, 0);
          const pct = Math.round((done/max)*100);
          const passed = msc.passed || isPassed(m, checks, reqs[m.id]||makeReq(m));
          return (
            <div key={m.id} onClick={() => setSel(m.id)} style={{ ...st.card, cursor:"pointer" }}>
              <div style={{ display:"flex", justifyContent:"space-between", alignItems:"center", marginBottom:6 }}>
                <div style={{ display:"flex", alignItems:"center", gap:8 }}>
                  <div style={{ width:7, height:7, borderRadius:"50%", background:m.color }} />
                  <div style={{ fontSize:14 }}>{m.label}</div>
                </div>
                <div style={{ display:"flex", alignItems:"center", gap:8 }}>
                  {passed && done > 0 && <Badge small />}
                  <div style={{ fontSize:13, color:m.color }}>{pct}%</div>
                </div>
              </div>
              <div style={{ height:3, background:pal.border, borderRadius:2, overflow:"hidden", marginBottom:5 }}>
                <div style={{ height:"100%", width:`${pct}%`, background:m.color, borderRadius:2 }} />
              </div>
              <div style={{ display:"flex", justifyContent:"space-between" }}>
                <div style={{ fontSize:11, color:pal.muted }}>{done}/{max}項目</div>
                {msc.evaluator ? <div style={{ fontSize:11, color:pal.gold }}>評価: {msc.evaluator}　{msc.date}</div> : <div style={{ fontSize:11, color:"#ccc" }}>未評価</div>}
              </div>
            </div>
          );
        })}
      </div>
    </div>
  );
}

function Manual() {
  const [sel, setSel] = useState(null);
  if (sel) return (
    <div style={st.app}>
      <div style={st.hdr}><button onClick={() => setSel(null)} style={{ ...st.btn("sm"), color:"#aaa", border:"1px solid #444" }}>← 戻る</button></div>
      <div style={{ padding:"24px 20px" }}>
        <div style={{ fontSize:10, color:pal.gold, letterSpacing:"0.15em", marginBottom:6 }}>CHAPTER {String(sel.no).padStart(2,"0")}</div>
        <div style={{ fontSize:18, marginBottom:6, lineHeight:1.5 }}>{sel.title}</div>
        <div style={{ fontSize:12, color:pal.muted, marginBottom:20 }}>{sel.sub}</div>
        <div style={{ fontSize:14, lineHeight:1.9, color:pal.accent, whiteSpace:"pre-line" }}>{sel.body}</div>
      </div>
    </div>
  );
  return (
    <div style={{ padding:"20px 16px" }}>
      <div style={st.label}>新卒スタッフ教育マニュアル</div>
      <div style={{ fontSize:12, color:pal.muted, fontStyle:"italic", marginBottom:20, lineHeight:1.8 }}>余分なものをそぎ落とし、本来の美しさを引き出す。</div>
      {CHAPTERS.map(ch => (
        <div key={ch.no} onClick={() => setSel(ch)} style={{ ...st.card, display:"flex", alignItems:"center", gap:14, cursor:"pointer" }}>
          <div style={{ fontSize:18, color:pal.border, minWidth:26 }}>{String(ch.no).padStart(2,"0")}</div>
          <div style={{ flex:1 }}><div style={{ fontSize:14, marginBottom:2 }}>{ch.title}</div><div style={{ fontSize:11, color:pal.muted }}>{ch.sub}</div></div>
          <div style={{ color:pal.border, fontSize:16 }}>›</div>
        </div>
      ))}
    </div>
  );
}

export default function App() {
  const [user, setUser] = useState(null);
  const [tab, setTab] = useState("checklist");
  const [scores, setScores] = useState({});
  const [sel, setSel] = useState(null);
  const [menus, setMenus] = useState(MENUS);
  const [reqs, setReqs] = useState(() => {
    const o = {};
    MENUS.forEach(m => { o[m.id] = makeReq(m); });
    return o;
  });

  const saveScore = (sid, mid, data) => setScores(p => ({ ...p, [sid]:{ ...(p[sid]||{}), [mid]:data } }));
  const handleReq = (mid, k, v) => setReqs(p => ({ ...p, [mid]:{ ...p[mid], [k]:v } }));
  const handleUpdateMenu = (mid, newSecs) => {
    setMenus(p => p.map(m => m.id !== mid ? m : { ...m, sections:newSecs }));
    setReqs(p => {
      const nm = menus.find(m => m.id === mid);
      return { ...p, [mid]:makeReq({ ...nm, sections:newSecs }) };
    });
  };

  if (!user) return <Login onLogin={u => { setUser(u); setTab(u.isAdmin?"admin":"checklist"); }} />;

  const tabs = user.isAdmin
    ? [{ id:"admin", label:"進捗管理" }, { id:"checklist", label:"チェックリスト" }, { id:"manual", label:"マニュアル" }]
    : [{ id:"checklist", label:"チェックリスト" }, { id:"manual", label:"マニュアル" }];

  return (
    <div style={st.app}>
      <div style={st.hdr}>
        <div style={st.logo}>NEUTRIZE</div>
        <div style={{ display:"flex", alignItems:"center", gap:10 }}>
          <div style={{ fontSize:11, color:"#aaa" }}>{user.name}</div>
          <button onClick={() => { setUser(null); setSel(null); }} style={{ ...st.btn("sm"), color:"#888", border:"1px solid #444", fontSize:11 }}>ログアウト</button>
        </div>
      </div>
      <div style={st.nav}>{tabs.map(t => <button key={t.id} onClick={() => { setTab(t.id); setSel(null); }} style={st.nb(tab===t.id)}>{t.label}</button>)}</div>
      {tab === "manual" && <Manual />}
      {tab === "checklist" && <MenuList user={user} scores={scores} onSave={saveScore} isAdmin={user.isAdmin} canEdit={user.canEdit||false} readOnly={!user.isAdmin} menus={menus} reqs={reqs} onReq={handleReq} onUpdateMenu={handleUpdateMenu} />}
      {tab === "admin" && !sel && <Dashboard scores={scores} menus={menus} reqs={reqs} onSelect={setSel} />}
      {tab === "admin" && sel && <StaffDetail staff={sel} user={user} scores={scores} onSave={saveScore} menus={menus} reqs={reqs} onReq={handleReq} onUpdateMenu={handleUpdateMenu} onBack={() => setSel(null)} />}
    </div>
  );
}
