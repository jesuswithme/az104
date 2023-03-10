# az-104에서 Lab 환경 구성을 위한 파일이다
# 환경 구성을 하는 방법은 다음과 같다.
# 먼저 git clone으로 다운로드 받는다
# cd az104
# cd Module04
# 다음과 같이 json 파일을 가져오면 된다
az group create --name devRG --location eastus
az deployment group create -g devRG --template-file az104-04-vms-loop-template.json --parameters az104-04-vms-loop-parameters.json
