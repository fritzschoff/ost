<script>
  export const numberOfWallets = () => {
    // Fetch wallets from API
    return 50;
  };
</script>

<div>
  powered by OST on Ethereum
  <br />
  +{numberOfWallets()}k wallets on layer-2
</div>

<style>
  div {
    width: 100%;
    max-width: 700px;
    margin-bottom: 60px;
    border-radius: 7px;
    background-color: #0598a0;
    box-shadow: 4px 4px 8px 2px rgb(0 0 0 / 21%);
    padding-top: 20px;
    padding-bottom: 20px;
    color: #fff;
    font-size: 36px;
    font-weight: 300;
    text-align: center;
  }
</style>
