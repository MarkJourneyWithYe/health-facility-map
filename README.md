# 전국 보건 시설 지도

전국건강생활지원센터(132개소) + 전국치매센터(317개소) 표준데이터를 카카오/외부 키 없이 단일 HTML로 시각화.

- **데이터:** 한국건강증진개발원 표준데이터 (공공데이터포털)
- **지도:** Leaflet 1.9 + OpenStreetMap 타일
- **디자인:** Pretendard Variable + JetBrains Mono, 크림 `#FAF7F2` + 1px 검정 보더

## 구성

- **A · 지도** — 449개 시설 마커(녹색=건강생활, 보라=치매), 클러스터링, 검색·필터·목록
- **B · 대시보드** — 시·도별 분포, 시설 유형, 평균 인력 구성, 장비/사업 보유율, 사업 분야 빈도

## 빌드

```bash
cd ..
python3 build_map.py
cp dashboards/facility_map.html deploy/index.html
```
