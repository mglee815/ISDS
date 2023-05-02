이 코드는 총 7개의 감정으로 짧은 텍스트를 분류하는 모델입니다.

감정의 종류는 
'공포', '놀람', '분노', '슬픔', '중립', '행복', '혐오'로 구성되어 있습니다.

학습에 사용한 데이터는
aihub에서 제공하는
<한국어 감정 정보가 포함된 단발성 대화 데이터셋>으로 
총 38,594 문장의 SNS글 및 온라인 댓글에 대하여 레이블링을 수행한 데이터셋입니다.
자세한 정보는 아래에서 확인하실 수 있습니다.
https://aihub.or.kr/mypage/reqst/datareqst/view.do?currMenu=157&topMenu=106&dataReqstSn=370150

분류 모델은 KoBERT를 기반으로 수행했으며
학습에 사용한 하이퍼파라미터는 아래와 같습니다.
{
num_epochs = 5
batch_size =16
max_len =128
learning_rate =5e-5
}

사용 방법은 example.ipynb 파일에 주석으로 설명해두었습니다.