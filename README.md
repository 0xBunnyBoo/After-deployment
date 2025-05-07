forge verify-contract \
    --chain-id 1301 \
    --num-of-optimizations 200 \
    --watch \
    --constructor-args $(cast abi-encode "constructor(string,string,uint256,uint256)" "ForgeUSD" "FUSD" 18 1000000000000000000000) \
    --etherscan-api-key {your_etherscan_api_key} \
    --compiler-version {v0.8.20+commit.a1b79de}
    {the_contract_address} \
    src/{YourContract}.sol:{ContractName}
