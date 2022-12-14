# Comfort by Default

Ranol☆P가 운영하는 Minecraft, Minecraft: Java Edition 서버입니다.
여러 플러그인을 사용해 편의성을 향상시켜 서바이벌 플레이의 피로도를 줄였습니다.

허용 목록에 등록된 사람만 서버에 접속할 수 있으며,
테러, 버그 악용, 서버에 불필요한 부하를 주는 행위나 기타 불쾌감을 주는 행위 등은 적발될 경우 차단당할 수 있습니다.

기본적으로 기능은 Minecraft: Java Edition을 기준으로 개발되어 있기 때문에
Bedrock Edition 클라이언트에서 이상하게 작동할 수 있습니다.
아래 표에 나온 기호를 참고해 기능을 살펴보시기 바랍니다.

| 기호      | 설명                          |
| --------- | ----------------------------- |
| :star:    | 호환됩니다.                   |
| :x:       | 호환되지 않습니다.            |
| :warning: | 호환성이 검증되지 않았습니다. |

## 삶의 품질을 높이는 기능 목록

- [x] 웹 지도 - [BlueMap](https://www.spigotmc.org/resources/bluemap.83557/) :star:
- [x] Java/Bedrock 에디션 동시 지원 - [Geyser](https://github.com/GeyserMC/Geyser) + [Floodgate](https://github.com/GeyserMC/Floodgate) :star:
- [x] 시체 회수 - [Graves](https://www.spigotmc.org/resources/graves.74208/) :star:
- [x] 상자 정리 - [ChestSort](https://www.spigotmc.org/resources/chestsort-api.59773/) :warning:
- [x] Discord 채팅 연동 - [DiscordSRV](https://www.spigotmc.org/resources/discordsrv.18494/) :star:
- [x] Bundle 레시피 제공 - 가죽 획득 시 해금됨 :x:
- [x] 50% 수면으로 밤 넘기기 :star:
- [x] 블록은 터트리지 않는 크리퍼 :star:
- [ ] 농사 편의성
  - [x] 경작지에서 뛰어다녀도 농작물이 짓밟히지 않음 - [SimpleNoCropTrample](https://www.spigotmc.org/resources/simplenocroptrample.73609/) :star:
  - [ ] 작물 수확으로 경험치 획득
  - [x] 다 자란 작물을 우클릭해 수확 - [RightClickHarvest](https://www.spigotmc.org/resources/rightclickharvest.84620/) :star:
- [x] 공중 나뭇잎 소거
- [x] 웨이포인트 지정 - [Waypoints](https://www.spigotmc.org/resources/waypoints.66647/) :warning:
- [ ] 귀환
  - [x] 모닥불에 시프트 우클릭해 집 지정 :star:
    - [x] 따스한 날갯짓 - 깃털 획득 시 해금됨, 소모 아이템 :star:
    - [x] 불꽃이 깃든 보석 - 자수정 획득 시 해금됨, 영구, 600초 쿨타임 :star:
  - [ ] Waystone
- [ ] 버림 방지
- [ ] Grappling Hook
- [ ] 쓰레기통
- [ ] 생명력 막대/피해 표시기
- [ ] WAILA
- [ ] Tips/Guide
- [ ] FindMe?
- [ ] Carry On
- [ ] Creative Flight
- [ ] Craftable Magics
- [ ] Artifacts
- [ ] Enchantments++
- [ ] Sleep -> Buff
- [ ] Healing Campfire
- [ ] Dynamic Light?
- [ ] Chunk Claim
- [ ] Teams
- [ ] Escape!
- [ ] Ultimine? Choptree?
- [ ] Hat
- [ ] Horse
- [ ] RPG-ish Combat
  - [ ] Parry
  - [ ] Dualwield
  - [ ] Roll
  - [ ] Wall-run
  - [ ] Wall Climb
- [ ] Travel Anchor
- [ ] Tiny Charcoal <- Disc Fragment
- [ ] Wither Skeleton Skull Fragment <- Dark Oak Button
- [ ] Summoning Altar
- [ ] Enchantment Extractor

## 관리자 보조 수단

- [x] 권한 관리 - LuckPerms
- [x] 블록 로그 확인 - CoreProtect

## 서버 실행

### 사전 요구 사항

- [asdf-vm](https://asdf-vm.com/)을 설치해주십시오. Java 런타임 관리를 위해 사용합니다.

### 설치

- `setup-runtime.sh`를 실행해 asdf 런타임을 깝니다.
- `setup-server.sh`를 실행해 서버 실행에 필요한 파일을 내려받습니다.
- `install.sh`를 실행해 systemd 서비스 파일을 생성해 배치합니다.
- `systemctl --user enable minecraft-vanilla`로 서비스를 활성화합니다.

### 시범 실행

- `run.sh`를 직접 실행해 서버를 실행해봅니다.

### 포트 정보

- Java Edition 서버: 25000 포트 - SRV 레코드를 활용해 25565 포트로 접속할 수 있습니다.
- Bedrock Edition 프록시: 19132 포트
- BlueMap 웹 서버: 25001 포트 - 리버스 프록시를 통해 443 포트로 HTTPS 접속이 가능합니다.
