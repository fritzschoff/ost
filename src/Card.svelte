<script lang="ts">
  import type { Card } from "./interfaces/card.interface";
  export const cards: Card[] = [
    {
      title: "Utility Tokens",
      description:
        "Issue tokens on layer-1 Ethereum, then settle transactions inside your application on layer-2. Define contract rules on how your token behaves within your app.",
      link: "see github",
      href: "https://github.com/openst/openst-contracts",
      backgroundColor: "hsla(255.1578947368421, 42.60%, 56.27%, 1.00)",
    },
    {
      title: "Wallet Recovery",
      description:
        "Integrate a self-custodial contract wallet SDK into your mobile app (iOS/Android). Support multiple devices and secure access recovery with a 6-digit PIN.",
      link: "see github",
      href: "https://github.com/OpenST/ost-wallet-sdk-android",
      backgroundColor: "hsla(337, 67.55%, 51.78%, 1.00)",
    },
    {
      title: "OST chain",
      description:
        "Move ERC20 tokens and messages securely between Ethereum chains with Merkle proofs. OST chain runs your EVM contracts on layer-2 for cheap gas costs.",
      link: "see github",
      href: "https://github.com/openst/mosaic-contracts",
      backgroundColor: " hsla(226, 83.34%, 62.11%, 1.00)",
    },
    {
      title: "OpenST Platform",
      description:
        "OpenST Platform provides a backend to relay meta-transactions signed by the user in your app to the OST chain. Pay for your users gas fees.",
      link: "see github",
      href: "https://github.com/openst/platform-api",
      backgroundColor: "hsla(88, 77.75%, 53.65%, 1.00)",
    },
  ];
</script>

<section>
  <span>CODE CONTRIBUTIONS</span>
  <h3>
    Your key, your coin, your data.
    <br />
    Simple to own, simple to recover.
  </h3>
  <div>
    {#each cards as card}
      <article style="background-color: {card.backgroundColor}">
        <h4>{card.title}</h4>
        <p>{card.description}</p>
        <a href={card.href}>{card.link}</a>
      </article>
    {/each}
  </div>
</section>

<style>
  section {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  span {
    opacity: 0.6;
    margin-bottom: 10px;
    font-size: 12px;
    line-height: 20px;
    font-weight: 500;
    letter-spacing: 1px;
    text-transform: uppercase;
  }

  h3 {
    text-align: center;
    margin-top: 10px;
    margin-bottom: 10px;
    font-size: 36px;
    line-height: 50px;
    font-weight: 400;
  }
  article {
    width: 300px;
    height: 300px;
    margin: 0px auto 30px;
    border-style: solid;
    border-width: 1px;
    border-color: rgba(207, 205, 205, 0.66);
    border-radius: 7px;
    background-color: transparent;
    box-shadow: 4px 4px 8px 2px rgb(0 0 0 / 21%);
  }
  div {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
  }
</style>
