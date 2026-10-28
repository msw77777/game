# 리르가드의 미궁 (The Catacombs of Lirgard)

위자드리풍 1인칭 던전 RPG. 브라우저에서 `index.html` 하나로 돌아간다.

- 캐릭터 생성(종족·능력치·직업), 4인 파티, 지하 3층 미궁, 마도왕 베르가스 토벌
- 턴제 전투, 주문, 버프·디버프(축복·보호·약화·저주·독), 전투 이펙트
- 마을: 의뢰 게시판, 여관(레벨업·저장), 상점, 사원
- 저장은 여관에서만 (기록부 3칸)
- 1인칭 고딕 마을: 시설을 고르면 걸어가서 시설 창(상점 구입·판매, 의뢰, 여관, 사원)이 열린다
- 미궁에서 M 키 또는 [지도 켜기]로 화면 위 반투명 지도

## 실행

`assets/manifest.json`을 읽어야 하므로 파일을 더블클릭하지 말고 간단한 웹 서버로 연다.

```
python3 -m http.server 8000
# 브라우저에서 http://localhost:8000
```

## 폴더

```
index.html          게임 본체
guide.html          그림 교체 가이드
assets/
  manifest.json     그림 목록 (경로·프레임 수·속도·도트 여부)
  CREDITS.txt       그림 출처와 라이선스
  party/            파티 초상 (warrior, thief, priest, mage)
  monsters/         몬스터 (slime … chort, boss)
  props/            보물상자
```

그림을 바꾸는 방법은 `guide.html`에 정리되어 있다. 같은 이름의 파일로 바꾸고, 프레임 수가 달라졌으면 `manifest.json`만 고치면 된다.

## 라이선스 (그림)

- 도트 캐릭터·몬스터·상자: 0x72 「16x16 DungeonTileset II」 — CC0 1.0
- 아이콘: game-icons.net (Lorc, Delapouite, Skoll, DarkZaitzev) — CC BY 3.0
