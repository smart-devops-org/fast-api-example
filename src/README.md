# github action + ecr + argocd 배포

1. ecr를 사용하기 위한 사용자 추가
   - iam에 사용자 추가
   - 정책 연결 AmazonEC2ContainerRegistryFullAccess
2. 콘솔 엑세스 활성화

   - 사용자 암호 지정

3. 인증을 위한 엑세스 키 설정

   - AWS 외부에서 실행되는 애플리케이션
   - access_key
   - private_access_key

4. ecr에 레포지토리 생성

5. 깃 레포 생성 및 시크릿 설정

-
