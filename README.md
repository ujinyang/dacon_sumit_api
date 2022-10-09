# dacon_sumit_api

DACON 사이트에서 사용하는 제출용 API package

# colab에서 설치
```notebook
!pip install https://raw.githubusercontent.com/ujinyang/dacon_sumit_api/main/dacon_submit_api-0.0.4-py3-none-any.zip
```

# 코드제출시 사용방법
```python
from dacon_submit_api import dacon_submit_api 

result = dacon_submit_api.post_submission_file(
'파일경로',             # ./data/submission.csv
'개인 Token',           # 계정정보에서 발급받아야 함.
'대회ID',               # 대회ID는 URL에 표시되는 숫자 (ex. AI 양재허브 인공지능 오픈소스 경진대회 : 235977 )
'팀이름',               # 팀이름 : basslibrary
'submission 메모 내용'  # Model 명 / Optimizer / LR / Epochs / loss, pnsr etc. 기입.
)

# 추후 검증을 위해 결과제출파일과는 별도로 소스파일 저장도 필요함.
# 백업을 안하더라도 저장만하면 google drive의 과거이력조회로 찾을 수는 있음.

```
