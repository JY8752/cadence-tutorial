# Cadence Tutorial 8. Marketplace Compose

## accountのセットアップ

```
flow transactions send cadence/transactions/SetupAccount1Transaction.cdc --signer default
flow transactions send cadence/transactions/SetupAccount2Transaction.cdc --signer account2 
```

## mint

```
flow transactions send cadence/transactions/SetupAccount1TransactionMinting.cdc --signer default
```

## check

```
flow scripts execute cadence/scripts/CheckSetupScript.cdc    
```

## 販売

```
flow transactions send cadence/transactions/CreateSale.cdc --signer default
```

## 販売ID確認

```
flow scripts execute cadence/scripts/GetSaleIDs.cdc
```

## 購入

```
flow transactions send cadence/transactions/PurchaseSale.cdc --signer account2
```

## 確認

```
flow scripts execute cadence/scripts/VerifyAfterPurchase.cdc
```