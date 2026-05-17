# 用語・記号一覧

ウェブハンドリングで頻出する用語と記号を一覧にまとめる。本サイト全体で共通に使用する。
出典：橋本 巨『入門 ウェブハンドリング』各章扉 KEY WORDS、橋本 巨『ウェブハンドリングの基礎理論と応用』第2章、『スリッター・リワインダーの技術読本』第1章他。

---

## 1. 基本概念

| 用語 | 英語 | 説明 |
|------|------|------|
| ウェブ | web | 連続した薄物材料の総称（フィルム、紙、金属箔、不織布等） |
| 連続紙 | continuous paper | ロール状の連続した紙 |
| ロール・ツー・ロール搬送 | roll-to-roll (R2R) | 巻出から巻取までの連続搬送方式 |
| ウェブハンドリング | web handling | ウェブの搬送・取り扱い技術 |
| コンバーティング | converting | 原反に価値を付与する加工（コーティング、ラミネート、印刷等） |
| ウェブスパン | web span | 隣接する2本のロール間のウェブ区間 |

??? question "演習: 基本用語"
    「コンバーティング（converting）」と「ウェブハンドリング（web handling）」の違いを一言で答えよ。

    ??? success "解答"
        **コンバーティング**は原反に価値を付与する加工（塗工・ラミネート・印刷等）。
        **ウェブハンドリング**はそれを実現するための搬送・取り扱い技術。
        コンバーティングが「何を作るか」、ウェブハンドリングが「どう運ぶか」に対応する。

## 2. 装置・ロール・補機

| 用語 | 英語 | 説明 |
|------|------|------|
| 巻出機 | unwinder / unwind stand | 原反ロールを巻き出す装置 |
| 巻取機 | rewinder / winder | 製品ロールを巻き取る装置 |
| アイドラロール | idler roll | 駆動を持たず、ウェブに従動するロール |
| ドライブロール | drive roll | サーボやインダクションモータで駆動するロール |
| ニップロール | nip roll | 2本のロールでウェブを挟み、滑りを防いで搬送するロール |
| ダンサロール | dancer roll | バネ・エアシリンダで支持され、張力変動を吸収するロール |
| ガイドロール | guide roll | 蛇行修正のために回転軸を傾けるロール |
| スプレッダロール | spreader roll | しわを伸ばすためのバナナロール／溝付きロール |
| バナナロール（エキスパンダロール）| bowed roll / expander roll | 弓状の軸で軸方向外向きに拡幅する受動ロール |
| 凹面ロール | concave spreader roll | 中央が細く両端が太い樽形ロール |
| スパイラル溝付きロール | spiral grooved roller | 螺旋溝で軸方向力を発生させる拡幅ロール |
| テンター | tenter | クリップ／ピンで両端を機械的に幅出しする大型装置 |
| クーラントロール（チルロール） | chill roll | ウェブを冷却する内部水冷ロール |
| サクションロール | suction roll | 穿孔＋負圧で密着搬送するロール |
| 静圧ロール | hydrostatic roller | エアを噴出して非接触でウェブを保持するロール |
| マクログルーブロール | macro-grooved roller | 軸方向の深い溝で空気を排出するロール |
| マイクログルーブロール | micro-grooved roller | 微細な粗面化で空気膜を破るロール |
| アキュムレータ（蓄積装置） | accumulator | スプライス時等にウェブを蓄え、停止せず搬送を継続する装置 |
| ライダロール | rider roll | 巻取ロール表面に当てるニップロール（エア排除） |
| ターレット | turret | 自動切替式の巻出／巻取機構 |

??? question "演習: ロールの分類"
    次のうち「駆動を持たないロール」はどれか。
    (a) ドライブロール  (b) アイドラロール  (c) ニップロール  (d) ダンサロール

    ??? success "解答"
        **(b) アイドラロール**。ウェブに従動して回転するだけで、駆動源を持たない。
        (a) ドライブロールはモータ駆動、(c) ニップロールは多くの場合駆動、(d) ダンサロールは張力変動吸収用で軸が可動。

## 3. 寸法・座標

| 記号 | 名称 | 意味 | 単位 |
|------|------|------|------|
| MD | Machine Direction | 流れ方向（長手） | — |
| TD / CD | Transverse / Cross (Machine) Direction | 幅方向 | — |
| ND / ZD | Normal / Z Direction | 厚さ方向 | — |
| $w$ | ウェブ幅 | TD方向の幅 | m, mm |
| $h$ | ウェブ厚さ | NDの厚み | μm, mm |
| $L$ | スパン長 | ロール間距離 | m |
| $D$ | ロール径 | ロールの外径 | mm |
| $R$ | ロール半径 | $R = D/2$ | mm |
| $\theta_w$ | 巻き付き角 | ウェブがロールに巻き付く中心角 | rad, deg |

??? question "演習: 巻き付き角の単位"
    巻き付き角 $\theta_w = 180°$ をラジアンで表すといくつか。オイラーの摩擦式で使う単位はどちらか。

    ??? success "解答"
        $180° = \pi \approx 3.14\,rad$
        オイラー式 $T_2/T_1 \le e^{\mu\theta}$ では **ラジアン** を使う。度数法を入れると指数の値が桁違いになる。

## 4. 力学量

| 記号 | 名称 | 意味 | 単位 |
|------|------|------|------|
| $T$ | 張力 | ウェブ全幅にかかる引張力 | N |
| $\sigma$ | 引張応力 | $\sigma = T/(w h)$ | Pa, MPa |
| $t$ | 単位幅張力（線張力） | $t = T/w$ | N/m |
| $V$ | 搬送速度 | ウェブの長手方向速度 | m/min, m/s |
| $\omega$ | ロール角速度 | rad/s | rad/s |
| $\mu$ | 摩擦係数 | ウェブとロール間 | — |
| $\mu_s$ | 静摩擦係数 | 静止状態の摩擦係数 | — |
| $\mu_k$ | 動摩擦係数 | 滑り中の摩擦係数 | — |
| $\mu_\text{eff}$ | 有効摩擦係数 | 空気膜等の影響を含めた実効摩擦係数 | — |
| $E$ | ヤング率 | 縦弾性係数 | Pa, GPa |
| $G$ | 横（剪断）弾性係数 | $G = E/[2(1+\nu)]$ | Pa, GPa |
| $\nu$ | ポアソン比 | 横／縦ひずみ比 | — |
| $\varepsilon$ | ひずみ（縦ひずみ） | $\varepsilon = (L'-L)/L$ | — |
| $\varepsilon'$ | 横ひずみ | $\varepsilon' = (W-W')/W$ | — |
| $\gamma$ | せん断ひずみ | $\gamma = \Delta/L = \tan\theta$ | — |
| $\sigma_Y$ | 降伏応力 | 弾性域上限 | MPa |
| $\sigma_B$ | 引張強さ | ネッキング点の最大応力 | MPa |
| $\sigma_{0.2}$ | 耐力（0.2% proof stress） | 永久ひずみ 0.2% に対応する応力。非鉄金属で使用 | MPa |
| $\rho$ | 密度 | 質量密度 | kg/m³ |
| $\eta$ | 粘度 | 流体粘度（空気 ≈ 1.8×10⁻⁵ Pa·s） | Pa·s |

橋本『基礎理論と応用』第2章2節「ウエブの力学特性」の記号体系に倣う。

??? question "演習: 記号の意味"
    次の記号は何を表すか答えよ。
    (a) $\sigma_{0.2}$  (b) $\mu_\text{eff}$  (c) $t = T/w$

    ??? success "解答"
        (a) **耐力**（0.2% proof stress、非鉄金属で降伏応力の代わりに用いる）
        (b) **有効摩擦係数**（空気膜等の影響を含めた実効値）
        (c) **単位幅張力**（線張力、N/m）

## 5. ウェブの変形モード

橋本『基礎理論と応用』第2章2節 図2-3 が示す基本的変形モード：

| モード | 英語 | 説明 |
|--------|------|------|
| 引張 | tension | MD 方向に引かれての伸び（および CD 縮み） |
| 圧縮 | compression | MD 方向に押されての縮み（および CD 伸び） |
| せん断 | shearing | 平行二辺がずれる変形 |
| 曲げ | bending | 曲げモーメントによるたわみ |
| ねじり | torsion | 端面ねじりによる軸まわりゆがみ |
| 座屈 | buckling | 圧縮で曲げ変形に転じる不安定現象 |

??? question "演習: 座屈の本質"
    「座屈」は他の変形モード（引張・圧縮・せん断・曲げ・ねじり）とどう本質的に異なるか。

    ??? success "解答"
        他は外力に対し連続的・安定的に変形するのに対し、**座屈は不安定現象**である。
        圧縮力がある臨界値を超えると、わずかな増加で急激にたわみ変形が成長する。
        しわは典型的な座屈現象で、CD圧縮応力が薄板座屈臨界値を超えたときに発生する。

## 6. 弾性・粘弾性・レオロジー

橋本『入門』第3章 KEY WORDS に頻出。

| 用語 | 英語 | 説明 |
|------|------|------|
| フックの法則 | Hooke's law | $\sigma = E\varepsilon$ |
| 弾性変形領域 | elastic deformation region | 除荷で元に戻る変形領域 |
| 塑性変形 | plastic deformation | 永久ひずみを残す変形 |
| 引張試験 | tensile test | 応力-ひずみ曲線を得る基本試験 |
| 応力-ひずみ曲線 | stress-strain curve | 引張試験で得る材料特性曲線 |
| 等方性 | isotropic | 方向に依らない物性 |
| 非等方性（異方性） | anisotropic | 方向によって物性が異なる |
| 鎖状配向フィルム | chain-oriented film | 高分子鎖が長軸方向に並んだフィルム |
| 面配向フィルム | planar-oriented film | 高分子鎖が面内に二次元配向 |
| 面配向・結晶化フィルム | planar-oriented crystalline film | 二軸延伸＋熱処理結晶化フィルム |
| 連続体モデル | continuum model | ウェブを連続体として扱うモデル |
| 分布定数モデル | distributed-parameter model | スパン内で物理量が空間分布するモデル |
| 集中定数モデル | lumped-parameter model | 質点・バネ・ダッシュポットで近似 |
| ニュートンの粘性法則 | Newton's law of viscosity | $\tau = \eta \dot\gamma$ |
| 粘弾性体 | viscoelastic body | 弾性と粘性を併せ持つ材料 |
| 力学モデル | mechanical model | バネ・ダッシュポットによる粘弾性表現 |
| 瞬間弾性ひずみ | instantaneous elastic strain | 応力印加直後の弾性ひずみ |
| クリープ | creep | 一定応力下でひずみが時間とともに増加する現象 |
| 応力緩和 | stress relaxation | 一定ひずみ下で応力が時間とともに減少 |
| 遅延弾性回復ひずみ | delayed elastic recovery strain | 除荷後ゆっくり回復する弾性ひずみ |
| 一般化フォークト・モデル | generalized Voigt model | 粘弾性のバネ・ダッシュポット並列モデル |
| 構成方程式 | constitutive equation | 応力とひずみの関係式の総称 |
| レオロジー | rheology | 物質の変形・流動を扱う分野 |

??? question "演習: クリープと応力緩和"
    プラスチックフィルムに張力をかけ続けると、徐々に伸びる。これは「クリープ」か「応力緩和」か。

    ??? success "解答"
        **クリープ**。一定応力下でひずみが時間とともに増加する現象。
        逆に、ひずみを固定した状態で応力が低下していくのが「応力緩和」。
        どちらもプラスチック・紙等の粘弾性材料で観察される。

## 7. 曲げ・座屈・しわ

| 用語 | 英語 | 説明 |
|------|------|------|
| ベルヌイ-ナビエの仮定 | Bernoulli-Navier hypothesis | 曲げ前後で断面の平面が保たれる仮定 |
| 断面の平面保持の仮定 | plane section hypothesis | 同上 |
| 中立面 | neutral plane | 曲げ時にひずみゼロの面 |
| 中立軸 | neutral axis | 中立面と断面の交線 |
| 曲げ剛性 | bending rigidity | $D = E h^3 / 12(1-\nu^2)$ |
| 線形座屈理論 | linear buckling theory | 中立安定条件から座屈荷重を求める |
| 非線形座屈理論 | nonlinear buckling theory | 座屈後の大変形を扱う |
| 長柱 | column | 断面寸法に比べ長さが極端に大きい棒 |
| 座屈限界値（座屈荷重） | critical buckling load | 座屈が始まる圧縮力 |
| 座屈応力 | buckling stress | 座屈荷重を断面積で除した値 |
| 座屈形 | buckling mode | 座屈直後のたわみ形状 |
| トラフ | trough | 波板状のくぼみ。折れしわの前駆形態 |
| 折れしわ | fold wrinkle | 永久痕の残る鋭い折れ込み |
| 臨界ミスアラインメント角度 | critical misalignment angle | 折れしわ発生の限界角度 |
| ポアソン効果 | Poisson effect | 引張方向と直交する縮み |
| カール | curl | ウェブが平らに戻らずに丸まる現象 |
| ラミネート加工 | lamination | 複数層を貼り合わせる加工 |
| 積層ウェブ | laminate web | 複数層からなるウェブ |
| 接着層 | adhesive layer | 積層ウェブの粘着剤層 |
| 線膨張係数 | linear expansion coefficient | $\alpha$、$\Delta L/L = \alpha \Delta T$ |
| 熱応力 | thermal stress | 熱膨張差で生じる内部応力 |

??? question "演習: トラフとしわの関係"
    「トラフ」と「折れしわ」の関係を述べよ。

    ??? success "解答"
        **トラフは折れしわの前駆形態**。ロールミスアラインメントによってウェブに波板状のくぼみ（トラフ）が発生し、これが下流ロール上で折れ込んで永久痕の **折れしわ** になる。
        トラフ段階で気付いて対策できれば、永久損傷は防げる。

## 8. 摩擦・トライボロジー

橋本『入門』第4章「ウェブハンドリングのトライボロジー」KEY WORDS より。

| 用語 | 英語 | 説明 |
|------|------|------|
| 最大静止摩擦力 | maximum static friction | 動き出し直前の摩擦力 |
| 静摩擦力 | static friction | 静止状態の摩擦力 |
| 動摩擦力 | kinetic friction | 滑り中の摩擦力 |
| 摩擦係数 | coefficient of friction | 摩擦力／垂直力 |
| アモントン-クーロンの摩擦法則 | Amontons-Coulomb's law | 摩擦力は垂直力に比例、接触面積に無関係 |
| オイラーのベルト公式 | Euler's belt equation | $T_2/T_1 = e^{\mu\theta}$ |
| 摩擦のメカニズム | friction mechanism | 凝着・掘り起こし等 |
| 摩擦の凝着説 | adhesion theory of friction | 真実接触点での凝着が摩擦の本質 |
| フラクタル性 | fractality | 粗面構造の自己相似性 |
| 表面粗さ曲線 | surface roughness profile | 触針式・光学式で得る粗さデータ |
| 触針式粗さ計 | stylus profilometer | 針で表面をなぞる粗さ計 |
| 走査型電子顕微鏡 | SEM | 電子線で表面を観察 |
| 共焦点レーザ顕微鏡 | confocal laser microscope | 焦点深度を利用した3D観察 |
| 走査型トンネル顕微鏡 | STM | トンネル電流で原子配列観察 |
| 原子間力顕微鏡 | AFM | 原子間力で表面を観察 |
| 粗さ突起 | asperity | 微視的な突起 |
| 真実接触面積 | real contact area | 突起同士が実際に接する面積 |
| ヘルツ接触 | Hertzian contact | 弾性体の点／線接触の古典理論 |
| 塑性指数 | plasticity index | $\psi$、弾性／塑性領域を判別 |
| 有効摩擦係数 | effective friction coefficient | 空気膜等を含めた実効摩擦係数 |
| 空気巻き込み（空気同伴） | air entrainment | ロール表面とウェブ間にエアが引き込まれる現象 |
| レイノルズ方程式 | Reynolds equation | 流体潤滑の支配方程式 |
| フォイル軸受理論 | foil bearing theory | 薄板と硬面間の弾性流体潤滑理論 |
| EHL（弾性流体潤滑）問題 | elasto-hydrodynamic lubrication | 弾性体接触＋流体膜の連成問題 |
| ストライベック曲線 | Stribeck curve | 速度と摩擦係数の関係曲線 |

??? question "演習: 有効摩擦係数"
    通常の「摩擦係数 $\mu$」と「有効摩擦係数 $\mu_\text{eff}$」の違いを答えよ。

    ??? success "解答"
        **摩擦係数 $\mu$**：固体同士の純粋な接触における係数（アモントン-クーロン則）。
        **有効摩擦係数 $\mu_\text{eff}$**：空気膜（空気巻き込み）による浮上・潤滑効果を含めた実効値。
        高速搬送では空気同伴で $\mu_\text{eff}$ が $\mu$ より大きく低下し、スリップの原因となる。

## 9. 蛇行・ガイド

橋本『入門』第7章 KEY WORDS より。

| 用語 | 英語 | 説明 |
|------|------|------|
| 蛇行 | wandering / lateral motion | ウェブが CD 方向に位置ずれする現象 |
| ウェブの直角方向進入性 | normal entry rule | ウェブは下流ロール軸に直角に進入する原理 |
| トラッキング能力 | tracking capability | ウェブが正しい位置を維持する性質 |
| ミスアライメント | misalignment | ロール軸の平行度ずれ |
| はりの曲げ理論 | beam bending theory | 蛇行解析にも応用される |
| EPC | Edge Position Control | エッジ位置一定制御 |
| CPC | Center Position Control | 中央位置一定制御（両エッジ検出） |
| LPC | Line Position Control | 任意のライン（印刷マーク等）一定制御 |
| ピボット型ガイドロール | pivot guide | 中央旋回式の蛇行修正ロール |
| パラレル型ガイドロール | parallel shifter | 平行移動式の蛇行修正ロール |
| ステアリング型ガイドロール | steering guide | 前後軸旋回式 |

??? question "演習: EPC, CPC, LPC の使い分け"
    幅変動するウェブに最適な制御方式は EPC, CPC, LPC のどれか。

    ??? success "解答"
        **CPC（Center Position Control）**。両エッジを検出して中央を維持するため、幅変動に強い。
        EPC は片エッジのみで幅変動に弱く、LPC は印刷マーク等の特徴線を維持する用途に向く。

## 10. 巻取・スリット

橋本『入門』第5章および『スリッター・リワインダーの技術読本』KEY WORDS より。

| 用語 | 英語 | 説明 |
|------|------|------|
| 中心駆動巻取（センタードライブ） | center drive winding | コア軸をトルク駆動 |
| 表面駆動巻取（サーフェイスドライブ） | surface drive winding | 表面ドラム駆動 |
| 併用駆動巻取（コンビネーションドライブ） | combination drive winding | 中心＋表面の併用 |
| ニップワインド | nip winding | 中心駆動＋ニップロール |
| TNT | Tension–Nip–Torque | 巻取品質を支配する三要素 |
| 巻取張力 | wound-on tension（ $T_w$ ） | 巻取部での張力指令 |
| WOT | Wound-On Tension | 巻取応力（実際にロールに残る応力） |
| テーパテンション | taper tension | 巻径増に応じて張力を下げる制御 |
| 層間圧力 | inter-layer pressure | 巻層間に働く圧縮圧 |
| 半径方向応力 | radial stress | 圧縮、巻取ロール内部の主応力の1つ |
| 接線方向応力 | tangential stress | 巻取ロール内部の主応力の1つ |
| 等方性ロール | isotropic roll | 半径方向・接線方向ヤング率が等しい仮定 |
| 異方性ロール | anisotropic roll | 実体に近い、半径方向ヤング率が低い |
| 非線形ヤング率 | nonlinear Young's modulus | 圧力依存の半径方向ヤング率 |
| Altmann の公式 | Altmann's formula | 等方性ロール内応力分布の解析解 |
| Hakiel モデル | Hakiel's model | 異方性・非線形を考慮した巻取応力モデル |
| 巻取方程式 | winding equation | 巻取応力の非線形2階常微分方程式 |
| 非線形2階常微分方程式 | nonlinear 2nd-order ODE | 巻取方程式の数学的分類 |
| 固巻き状態 | fully compressed state | 層間に空気膜が残らない巻取状態 |
| 軟巻き状態 | not fully compressed state | 空気膜を含む緩い巻取状態 |
| 積極駆動 | active drive | 動力でロールを回す方式 |
| 消極駆動 | passive drive | ウェブ張力で従動する方式 |
| テンションカット | tension cut | ニップ等で上下流の張力を分離 |
| スリッタ | slitter | ウェブを長手方向に分割切断する装置 |
| シアーカット | shear cut | 上下刃のせん断による切断 |
| レザーカット | razor cut | カミソリ刃で切る方式 |
| スコアーカット | score cut | 刃を上から押し当てる方式 |
| ターレット | turret | 自動切替式の巻出／巻取機構 |

??? question "演習: TNT と巻取品質"
    巻取品質を支配する三要素「TNT」とは何か。

    ??? success "解答"
        **T**ension（巻取張力）／**N**ip（ニップ荷重）／**T**orque（中心トルク）。
        この3要素が巻取ロール内部の半径方向・接線方向応力分布を決定し、テレスコープ・スター欠陥・しわなどの巻取不良の発生有無を支配する。

## 11. 制御・信号

橋本『基礎理論と応用』第8章、『入門』第6章 KEY WORDS より。

| 記号・用語 | 英語 | 説明 |
|------------|------|------|
| PID | Proportional-Integral-Derivative | 比例・積分・微分制御 |
| P 制御 | proportional control | 比例制御。オフセット残存 |
| PI 制御 | PI control | 比例＋積分。オフセットゼロ |
| PID 制御 | PID control | 比例＋積分＋微分。応答改善 |
| 比例ゲイン $K_p$ | proportional gain | 比例項のゲイン |
| 積分ゲイン $K_i$ | integration gain | 積分項のゲイン |
| 微分ゲイン $K_d$ | derivative gain | 微分項のゲイン |
| 積分時間 $T_i$ | integration time | $K_p/K_i$ |
| 微分時間 $T_d$ | derivative time | $K_d/K_p$ |
| 比例要素 | proportional element | $G_c(s) = K_p$ |
| 最終値の定理 | final value theorem | $\lim_{t\to\infty} y(t) = \lim_{s\to 0} sY(s)$ |
| ラプラス変換 | Laplace transform | 時間→s 領域変換 |
| ラプラス逆変換 | inverse Laplace transform | s→時間 領域変換 |
| Heaviside の展開定理 | Heaviside expansion theorem | 部分分数展開による逆変換 |
| 伝達関数 | transfer function | 入出力比 $Y(s)/U(s)$ |
| ブロック線図 | block diagram | 制御系の図的表現 |
| フィードフォワード（FF） | feed-forward | 外乱推定値に基づく前向き補償 |
| フィードバック（FB） | feed-back | 偏差に基づく補正 |
| 固有振動数 $\omega_n$ | natural frequency | 2次系のパラメータ |
| 減衰比 $\zeta$ | damping ratio | 2次系のパラメータ |
| オーバーシュート | overshoot | 立ち上がり時の行き過ぎ |
| チューニング | tuning | ゲイン調整 |

??? question "演習: P と PI の違い"
    P 制御と PI 制御の決定的な違いは何か。

    ??? success "解答"
        **オフセット残存の有無**。
        P 制御では定常状態でも偏差（オフセット）がゼロにならない。
        PI 制御は積分項により、時間とともにオフセットがゼロに収束する。
        張力制御では必ず PI 以上が必要。

## 12. ウェブの欠陥・トラブル

| 用語 | 英語 | 説明 |
|------|------|------|
| しわ | wrinkle | ウェブが面外に局所座屈した状態 |
| 折れしわ | fold wrinkle | 永久痕の残る鋭いしわ |
| センタしわ | center wrinkle | 中央部の縦方向しわ |
| エッジしわ | edge wrinkle | 両端付近の縦方向しわ |
| バギング | bagging | 幅方向に伸びムラ・たるみが残る |
| 蛇行 | wandering / lateral motion | CD方向の位置ずれ |
| テレスコープ | telescoping | 巻取ロールが軸方向にずれ落ちる不良 |
| スターリング | starring | 巻取ロール端面に星形のしわ |
| ダイシング | dishing | 巻取ロール端面が皿状にずれる不良 |
| ブロッキング | blocking | 巻取ロール内でウェブ同士が貼り付く |
| カール | curl | ウェブが丸まる現象 |
| ゲージバンド | gauge band | 厚さムラが巻き重なって生じる帯状の盛り上がり |
| マクロスリップ | macro-slip | ロール全体で起こる巨視的滑り |
| ピンホール | pinhole | 微小な貫通孔 |
| ピッキング | picking | 塗工面が剥がれる現象 |
| ブリスタ | blister | ウェブ層間の膨れ・剥離 |
| ニップしわ | nip wrinkle | ニップ通過時に発生するしわ |
| バーストロール | burst roll | 過張力で巻取ロールが破断 |
| ルーズロール | loose roll | 緩い巻取で形状崩れ |

??? question "演習: 巻取不良の判別"
    巻取ロールが軸方向にずれ落ちる不良を何と呼ぶか。原因は半径方向応力の何が原因か。

    ??? success "解答"
        **テレスコープ（telescoping）**。
        半径方向応力が **過度に低い**（つまり層間摩擦力不足）ことが原因で、ウェブ間でスリップが生じることで発生する。
        対策はテーパテンション、ニップ追加、巻取張力プロファイルの最適化など。

## 参考

- 橋本 巨『入門 ウェブハンドリング』全7章, 加工技術研究会, 2010. 各節扉に KEY WORDS リスト。
- 橋本 巨『ウェブハンドリングの基礎理論と応用』第2章「ウェブハンドリングに関する基本的事項」, 加工技術研究会.
- 『スリッター・リワインダーの技術読本』第1章「基礎」.
- D. R. Roisum, *The Mechanics of Web Handling*, TAPPI Press, 1996（英語用語の対応）.
