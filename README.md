# remohardsw
Remote Hardware Switching System (RHSS)

サーバーなどがソフトウエア上の入力を受け付けなくなった場合に独立したハードウエアからリモートでターゲットサーバーの電源を物理的に操作する仕組みの構築


必要環境
1.RHSSへアクセス可能なネットワーク
2.RHSSへの電源供給

RHSSの構成
独立したハードウエアかつセキュアなネットワーク接続が可能な小型サーバー
ハードウエアスイッチ（リレー）をコントロール可能なIO

Raspberry Pi 3 or 4
Raspberry Pi用リレーシールド of GPIOでのコントロールが可能なリレーユニット
オプション RS-232C

MyTerminal <-ssh-> Raspberry Pi <-GPIO-> リレーユニット <-> マザーボード上のReset,Powerスイッチ

