# RESPONSE CODES

The folllowing response status codes are specific to the VyaPay Gateway.

| Status | Code | Description |
| --- | --- | --- |
| SUCCESS | 00  | The transaction has been accepted and approved by the host processor |
| PENDING | 01  | Call issuer for authorization |
| DECLINED | 02  | The transaction has been accepted but declined by the host processor |
| DECLINED | 03  | Request formatting error. Typically this error is received when missing required parameter values. The transaction was not passed to the host processor. |
| DECLINED | 04  | Confiscate card (no fraud assumed) |
| DECLINED | 05  | Do not honor card |
| DECLINED | 06  | A duplicate `vyalynk-idempotent-key` header value was detected. The transaction was not passed to the host processor. |
| DECLINED | 07  | The card passed for a level 3 transaction is not qualified. The transaction was not passed to the host processor. |
| PENDING | 08  | Valid ID required for transaction |
| DECLINED | 09  | Non-specified Error. You can try the transaction again |
| DECLINED | 10  | Approved for lesser amount |
| DECLINED | 11  | Invalid Account format |
| DECLINED | 12  | Transaction type not permitted for this account |
| DECLINED | 13  | Invalid transaction amount |
| DECLINED | 14  | Account number or length error. |
| DECLINED | 15  | Invalid issuer. |
| DECLINED | 17  | Cardholder requested a cancellation on recurring charges |
| DECLINED | 18  | Customer dispute |
| DECLINED | 19  | Bad transaction data or setup, re-enter |
| DECLINED | 20  | Void no longer possible, issue a refund |
| DECLINED | 21  | Invalid refund transaction, issue a void |
| DECLINED | 22  | Violation |
| DECLINED | 24  | PIN tries exceeded |
| DECLINED | 30  | Date error. Check format or value is a future date |
| DECLINED | 31  | Card type not accepted by host / switch |
| DECLINED | 34  | Confiscate card (fraud assumed) |
| DECLINED | 40  | Requested function not supported |
| DECLINED | 41  | Confiscate card (reported lost) |
| DECLINED | 43  | Confiscate card (reported stoled) |
| DECLINED | 44  | Try lesser amount |
| DECLINED | 51  | Insufficient funds |
| DECLINED | 54  | Credit/Debit card expired |
| DECLINED | 55  | Bad Debit/ EBT pin info |
| DECLINED | 56  | Invalid Address |
| DECLINED | 57  | Card not permitted for this transaction type |
| DECLINED | 59  | Card billing zip code is required for keyed in transactions |
| DECLINED | 60  | Invalid Zip/Postal code |
| DECLINED | 61  | Exceeds withdrawal limit |
| DECLINED | 62  | Invalid service code |
| DECLINED | 63  | Security violation |
| DECLINED | 65  | Exceeds activity limit |
| DECLINED | 70  | Terminal does not support card type |
| DECLINED | 72  | Account closed |
| DECLINED | 73  | Capture already processed |
| DECLINED | 74  | Refund / Void already processed |
| DECLINED | 76  | Record not found |
| DECLINED | 81  | Encryption Error (usually debit/ebt) |
| DECLINED | 82  | CVV incorrect |
| DECLINED | 84  | 3DS data incorrect |
| DECLINED | 89  | Bad merchant ID |
| DECLINED | 94  | Duplicate batch number |
| DECLINED | 96  | System error |
| DECLINED | 97  | CVV2 / CID error |
| DECLINED | 99  | Void not accepted |
| DECLINED | N3  | Cash back services unavailable (VISA) |
| DECLINED | N4  | Too much cash back (VISA) |
| DECLINED | N7  | CVV2 mismatch (VISA) |