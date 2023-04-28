<template>
  <main>
    <px-header :links="links" />

    <router-view class="container px-5 sm:px-20 py-20 flex justify-center" />
  </main>
</template>

<script>
import PxHeader from '@/components/PxHeader'
export default {
  name: 'app',
  components: {PxHeader},
  data() {
    return {
      links: [
        {
          title: 'BTC',
          to: {name: 'coin-detail', params: {id: 'bitcoin'}},
        },
        {
          title: 'ETH',
          to: {name: 'coin-detail', params: {id: 'ethereum'}},
        },
        {
          title: 'USDT',
          to: {name: 'coin-detail', params: {id: 'Tether'}},
        },
        {
          title: 'BNB',
          to: {name: 'coin-detail', params: {id: 'BNB'}},
        },
        {
          title: 'USDC',
          to: {name: 'coin-detail', params: {id: 'USD Coin'}},
        },
        {
          title: 'XRP',
          to: {name: 'coin-detail', params: {id: 'XRP'}},
        },
        {
          title: 'ADA',
          to: {name: 'coin-detail', params: {id: 'Cardano'}},
        },
        {
          title: 'STETH',
          to: {name: 'coin-detail', params: {id: 'Lido Staked ETH'}},
        },
        {
          title: 'DOGE',
          to: {name: 'coin-detail', params: {id: 'Dogecoin'}},
        },
        {
          title: 'MATIC',
          to: {name: 'coin-detail', params: {id: 'Polygon'}},
        },
        {
          title: 'SOL',
          to: {name: 'coin-detail', params: {id: 'Solana'}},
        },
        {
          title: 'DOT',
          to: {name: 'coin-detail', params: {id: 'Polkadot'}},
        },
        {
          title: 'LTC',
          to: {name: 'coin-detail', params: {id: 'Litecoin'}},
        },
        {
          title: 'BUSD',
          to: {name: 'coin-detail', params: {id: 'Binance USD'}},
        },
        {
          title: 'SHIB',
          to: {name: 'coin-detail', params: {id: 'Shiba Inu'}},
        },
        {
          title: 'TRX',
          to: {name: 'coin-detail', params: {id: 'TRON'}},
        },
        {
          title: 'AVAX',
          to: {name: 'coin-detail', params: {id: 'Avalanche'}},
        },
        {
          title: 'DAI',
          to: {name: 'coin-detail', params: {id: 'Multi Collateral DAI'}},
        },
        {
          title: 'WBTC',
          to: {name: 'coin-detail', params: {id: 'Wrapped Bitcoin'}},
        },
        {
          title: 'LINK',
          to: {name: 'coin-detail', params: {id: 'Chainlink'}},
        },
      ],
    }
  },
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
