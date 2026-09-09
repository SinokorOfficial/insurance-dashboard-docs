# 보험증권 취합 대시보드 · 개발 문서

장금그룹 해상보험 증권·보험료 취합 대시보드의 **공개 개발 문서**입니다.

- 문서 사이트: <https://sinokorofficial.github.io/insurance-dashboard-docs/>
- 코드 리포(비공개): <https://github.com/SinokorOfficial/insurance-dashboard>

## 공개 범위

아키텍처·업무 규칙·데이터 모델·판독 로직 등 **개발 이해에 필요한 내용**만 다룹니다.

다음은 **포함하지 않습니다.**

- 운영 시크릿, 계정, 연결문자열
- 인프라 리소스명 — IP·공유폴더명·VNet/서브넷·게이트웨이·레지스트리
- **실제 보험료·부보금액 등 영업 정보**
- 개인 이메일·연락처

## 로컬에서 보기

```bash
pip install -r requirements.txt
mkdocs serve          # http://127.0.0.1:8000
```

## 배포

`main` 브랜치의 `docs/**`, `mkdocs.yml`, `requirements.txt` 가 바뀌면
GitHub Actions 가 자동으로 빌드해 GitHub Pages 에 올립니다.

빌드는 `--strict` 로 돌기 때문에 **깨진 링크가 있으면 실패**합니다.
