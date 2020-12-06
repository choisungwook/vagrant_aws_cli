# 1. vagrant_aws_cli
vagrant를 이용한 aws_cli, eksctl 환경 구축

# 2. aws-configure 성공
* 명령어 실행시 오류 메세지가 없으면 성공
```sh
aws sts get-caller-identity
```
# 3. eksctl을 이용한 cluster 생성
```sh
eksctl create cluster \
--name demo1 \
--version 1.18 \
--region ap-northeast-2 \
--nodegroup-name demo-nodegroup1 \
--node-type t2.micro \
--nodes 1
```

# 참고자료
* 공식문서-aws-cli: https://docs.aws.amazon.com/ko_kr/cli/latest/userguide/install-cliv2-linux.html
* 공식문서-eksctl: https://docs.aws.amazon.com/ko_kr/eks/latest/userguide/getting-started-eksctl.html
* 블로그-eks IAM role: https://blog.naver.com/jd0909/221997514307
* 공식문서-aws cli IAM 설정: https://docs.aws.amazon.com/ko_kr/cli/latest/userguide/cli-configure-role.html