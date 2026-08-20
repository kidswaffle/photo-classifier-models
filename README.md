# photo-classifier-models

사진분류시스템 앱(영유아 사진 자동 분류)이 첫 실행 시 다운로드하는 대용량
ML 모델 자산 호스팅 전용 저장소. 소스코드는 없음 — Release 자산만 사용.

InsightFace `buffalo_l`이 자체 CDN에서 첫 실행 시 자동 다운로드되는 것과
동일한 패턴을 이 저장소로 재현한다(포터블 DMG 용량을 작게 유지하기 위해
대용량 모델은 앱 번들에 넣지 않고 런타임에 다운로드·캐싱).

## Releases

- **adaface-ir101-webface12m-v1**: mk-minchul/AdaFace(MIT License)
  IR-101/WebFace12M 체크포인트를 ONNX로 변환한 파일. 변환 스크립트는
  사진분류시스템 저장소의 `scripts/adaface_export/export_adaface_model.py`.
