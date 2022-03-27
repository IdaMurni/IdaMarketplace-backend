<h3 align="center">Official IdaMarketplace-Backend</h3>

<p align="center">
  <img src="https://github.com/IdaMurni/website/blob/main/src/assets/img/ida_murni_master.png" width="200"/>
</p>


Test Purposes available in Mumbai Testnet
```shell
export const nftAddress = '0x0A300802F475d248F3249aDe88B53d6ceBA01bEb';
export const nftMarketAddress = '0x27289580F7cBa32A1A83F4E123232E68Bc2381De';
```

Try running some of the following tasks:

Install all dependencies
```shell
yarn
```

run app
```shell
yarn dev
```

<p>
    How to use Auction: 
    <ul>
        <li>filled 3 parameter to the fields: _NFT, _NFTID, _STARTINGBID before you deployed the Auction Contract</li>
        <li>once it is deployed, call approve(auction_id, _NFTID) function from NFT.sol</li>
        <li>defined Auction time period. by setting we have 2, 7, 10, 15 days. for testing purpose we've set to 1Minute because we don't wat to wait until a couple days to get the result. see on </li>
        ```shell
            enum TimeDuration {
                OneMinute, // <- testing purpose
                Twentyfour,
                Seven,
                Ten,
                Fifteen
            }
        ```
        <li>once it set we will able to bit the Acution.</li>
        <li>drink coffee while waiting the bits is end!!</li>
    </ul>
<p>

| parameter    | type    | description                 |
|--------------|---------|-----------------------------|
| _NFT         | address | contract address of the NFT |
| _NFTID       | unit256 | the id of the NFT           |
| _STARTINGBID | uint256 | value                       |