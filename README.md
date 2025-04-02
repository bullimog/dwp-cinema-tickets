# cinema-tickets

## Description
The ticket purchaser declares how many and what type of tickets they want to buy.
Multiple tickets can be purchased at any given time.
Only a maximum of 25 tickets that can be purchased at a time.
Infants do not pay for a ticket and are not allocated a seat. They will be sitting on an Adult's lap.
Child and Infant tickets cannot be purchased without purchasing an Adult ticket.

| Ticket Type  | Price      |
|--------------|------------|
| INFANT       | £0         |
| CHILD        | £15        |
| ADULT        | £25        |

This Java service can be invoked to process cinema ticket purchases.
Each request consists of:
* accountId (Long)
* An Array of TicketTypeRequest

TicketTypeRequest comprises:
* Type (an enumerated value)
  * ADULT
  * CHILD
  * INFANT
* numberOfTickets(integer)


## Local building and testing
```
> mvn clean test
```

Entry point into service is:
* uk.gov.dwp.uc.pairtest.TicketPriceService
