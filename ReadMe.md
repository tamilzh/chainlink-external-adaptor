cd chainlink-adaptor/
npm run startServer -  To start the server
npm run stopServer - TO stop the server

Usage
*****

curl -X POST -H "content-type:application/json" "http://localhost:8082/" --data '{ "id": 1, "data" :{"chain": "P", "method": "platform.getCurrentSupply","params": {} }}'

curl -X POST -H "content-type:application/json" "http://localhost:8081/" --data '{ "id": 1, "data" :{"chain": "C", "method": "eth_getAssetBalance","params": ["0x8723e5773847A4Eb5FeEDabD9320802c5c812F46", "latest", "3RvKBAmQnfYionFXMfW5P8TDZgZiogKbHjM8cjpu16LKAgF5T"] }}'

curl -X POST -H "content-type:application/json" "http://localhost:8081/" --data '{ "id": 1, "data" :{"chain": "P", "method": "avm.getAllBalances","params": {"address":"X-avax1c79e0dd0susp7dc8udq34jgk2yvve7haclsz5r"} }}'

