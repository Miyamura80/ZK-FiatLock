# ZK-FiatLock
💱 Fiat-P2P Physical Goods Exchange protocol. 

How to take out the marketplace middlemen in exchange of Physical Goods <-> Money? Building P2P Marketplaces, removing value-extracting trusted 3rd-parties.

✅ This is possible with smart contracts today
❌ But average users don't use/trust crypto payments, leading to cold start problems

Solution: ZK-FiatLock
✨ Fiat-only UX, all crypto backend abstracted away for the users. This greatly reduces cold start problems, making it easy to onboard buy-side of the market. 
🙌 Eliminating prohibitive middlemen fees in the transaction
🏪 Unlocks Smooth fiat-UX P2P marketplaces: e.g. P2P Airbnb, P2P Amazon/Ebay, P2P Uber.

# Implementation

This project uses ZKP2P + ZKEmail to enable P2P fiat transactions, where buy-side only ever interfaces with fiat to buy physical goods/services. This is enabled by the following components:

1) Staking with fiat - uses ZKP2P in the backend to enable fiat staking on smart contracts, without ever needing a crypto wallet. Instead of ZKP2P used to do on-ramp vs off-ramp, ZKP2P is used to "stake" on smart contracts with fiat, using USDC as the backend 
2) QR-Code Scanning - to verify that access to a given lockbox has been granted, it uses QR-code scanning to finalize the transaction and end the dispute resolution, returning each of the stakes
