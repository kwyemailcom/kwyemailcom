## Geth 실행: 

geth는 path 걸어놨음으로 그냥 cmd 창에서 아래 명령을 넣으면 됩니다. 새 하드 설치하면 경로 바꿔서 다시 올리겠습니다. 

geth --http --http.addr "0.0.0.0" --http.port 8549 --datadir="E:\Ethereum\data" --authrpc.jwtsecret E:\Ethereum\consensus\prysm\jwt.hex console

## Beacon Chain 실행: 

prysm.bat 있는 디렉토리에서 실행하면 됩니다. 새 하드 설치하면 경로 바꾸서 다시 올리겠습니다. 

.\prysm.bat beacon-chain --execution-endpoint=http://localhost:8551 --jwt-secret=E:\Ethereum\consensus\prysm\jwt.hex --p2p-host-ip "211.219.37.226" --suggested-fee-recipient=0x01234567722E6b0000012BFEBf6177F1D2e9758D9
