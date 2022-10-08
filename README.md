# dacon_sumit_api

DACON 사이트에서 사용하는 제출용 API package

# colab에서 설치
!pip install https://raw.githubusercontent.com/ujinyang/dacon_sumit_api/main/dacon_submit_api-0.0.4-py3-none-any.zip

# 사용방법
from dacon_submit_api import dacon_submit_api 

result = dacon_submit_api.post_submission_file(
'파일경로', 
'개인 Token', 
'대회ID', # 대회ID는 URL에 표시되는 숫자
'팀이름',
'submission 메모 내용' )
