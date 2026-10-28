# 인덕션 컬러 매칭 (대리점 영업용)

QR로 들어와 제품 모델을 고르고, 상판·하부장·벽면 컬러를 바꿔 가며 인덕션과의 매칭을 비교하는 웹앱입니다.
서버나 빌드 과정 없이 `index.html` 한 파일로 동작합니다.

## 사용법
- 주소 뒤에 `?model=m1` 또는 `#m1`을 붙이면 해당 모델이 선택된 상태로 열립니다. (모델별 QR에 사용)
- 태블릿 가로 화면 기준으로 설계했습니다.

## GitHub Pages로 배포하기
1. GitHub에서 새 저장소를 만듭니다.
2. 이 폴더의 파일(`index.html`, `README.md`, `.nojekyll`)을 저장소에 올립니다.
3. 저장소의 Settings → Pages에서 Source를 `Deploy from a branch`, Branch를 `main` / `(root)`로 지정하고 저장합니다.
4. 몇 분 뒤 `https://<계정명>.github.io/<저장소명>/` 주소로 열립니다.

주의: GitHub Pages 주소는 주소를 아는 누구나 열 수 있습니다. 미공개 제품 이미지나 내부 자료는 올리기 전에 공개 가능 여부를 확인하세요.

## 데이터 수정 위치 (`index.html`의 `<script>` 안)
- `MODELS`: 제품 모델 (이름, 각도별 이미지, 블랙 이미지)
- `TOPS`, `CABS`, `WALLS`: 상판, 하부장, 벽면 옵션 (`img`/`thumb`에 이미지 지정 가능)
