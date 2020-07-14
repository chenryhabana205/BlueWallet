# bc-ur
This library is an implementation of [bc-ur](https://github.com/BlockchainCommons/Research/blob/master/papers/bcr-0005-ur.md).

Still in development, please do not use it in production;

## Install

```
yarn add bc-ur
```

## Usage

```
const {encodeUR, decodeUR} from 'bc-ur';

const hexstr = '7e4a61385e2550981b4b5633ab178eb077a30505fbd53f107ec1081e7cf0ca3c0dc0bfea5b8bfb5e6ffc91afd104c3aa756210b5dbc5118fd12c87ee04269815ba6a9968a0d0d3b7a9b631382a36bc70ab626d5670b4b48ff843f4d9a15631aa67c7aaf0ac6ce7e3bff03b2c9643e3375e47493c4e0f8635329d66fdec41b10ce74dcbf25fc15d829e7830c325643a98561f441b40a02e8353493e6afc16192fe99d90d8ca65539af77ddeaccc8943a37563a9ba83675bd5d4da7c60c9a172cf6940cbf0ec8fe04175a629932e3512c5d2aaea3cca3246f40a21ffdc33c3987dc7b880351230eb3759fe3c7dc7b2d3a20a95996ff0b7a0dba834f96beb64c14e3426fb051a936ba41569ab99c0066a6d9c0777a49e49e6cbad24d722a4c7da112432679264b9adc0a8cff9dd1fe0ee9ee2747f6a68537c389a7303a1af23c534ee6392bc17b04cf0fbce7689e66b673a440c04a9454005b0c76664639113458eb7d0902eff04d11138ce2a8ee16a9cd7c8926514efa9bd83ae7a4c139835f0fe0f68c628e0645c8524c30dfc314e825a7aa13224d98e2f7a9d12183a999bb1f28549c99a9072d99c05c24e0c84848c4fc147a094ab7b69e9cbea86952fccf15500fbb234ffe6ee6e6ded515c8016cb017ba36fb931ef276cec4ed22c1aed1495d2df3b3ce66c03f5b9ffa8434bf0e8fb149de94e050b3da178df1f76c00a366cb2801fabdf1a1e90cd3cd45ecb7a930a40b151455f76b726d552f31c21324992da257ff8bde2923dfd5d0d6b87233fae215ffacbecd96249099e7e3427d533db56cdb09c7475b4ce3314e33f43953a7370866cc11d85f00b71b15510b46c4b4fa490c660ddfeda0ceb1b8265995f7071c155ad1b57465fdc0fa81a73f9f19ac4872029d5844c1838f732e803043673e26cbc5b51297a324ff00a2d2d4222bad556b93d27c8e376e3ff8f9d37b3073410708ebb3d4dd7473d27212310b71a3c33a5c8f87f44824640e7f8970f4eda9364195c87a91172b8f085f1773641dde1ce21938746234055bc971ce2325f814e3eec60f781dd4faf52afd5be4a6b38656f7e9739f724cb7ccd4e4d01e802add3dc7b83191f894b3ee0ed752ee514d5ec55';

const fragments = encodeUR(hexstr, 500);

const payload = decodeUR(fragments);
```