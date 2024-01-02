Introduction

While creating CDS views, must be differentiated between customer and SNAP. Identification can be done using following sequence.
Is CDS view copied from SNAP CDS view database? If yes, then follow SNAP naming standard. 
Is CDS view logic introduced by Madiba team using SNAP knowledge then customized specific to client functionality? If yes, then follow SNAP name space.
Is CDS view copied from SAP standard view? If yes, then follow Customer naming standard.
Is CDS view logic built for customer functionality from starting? If yes, then follow Customer naming standard.

Packages
ZSNAP – Use this package for all SNAP naming standard objects.
ZBW – Use this for all ADSOs
ZATR – Use this for all ATR packages

Customer CDS Views Naming Conversion
•	Naming Standards:
  ZAAA_CCCCCCCCCCC - (SQL Name: ZAAACCCCCCCCCC)
  AAA is for Module
•	Modules AAA
  ZAAA (ZAAA_#####): Examples
  ZATR: Account to Report
  ZPTM: Plan to Make
  ZOTC: Order to Cash
•	Free name space CCCCCCCCCCCC
  Free name space – can be used based on functionality of view.

SNAP CDS Views Naming Convention
•	Naming standards:
  ZSNAP_AAABBCCC - (SQL Name: ZIAAABBCCC)
  AAA is for Module
  BB is for Functional Stack
  CCC is for Technical Layer
•	Modules AAA
  ZSNAP (ZSNAP_AAA#####): Examples
  ZSNAP_FAP: Accounts Payable
  ZSNAP_FAR: Accounts Receivable
  ZSNAP_FIN: Finance
  ZSNAP_OTC: Sales 
•	Stack numbers BB:
  If the first number after the stack is 0, then it is generic to the stack
  FIN00###: Generic
  FIN17### Product Costing
  FIN18###: PII Profit in Inventory 
  FIN180##: Acquisition/Config layer
  FIN182##: P&L
  FIN183##: Inventory
  FIN184##: Valuation
  FIN185##: Production/Tolling variances
  FIN187##: Integrated Fact tables
  FIN188##: Cubes
  FIN76###: FINEX Finance Extended
  FIN19###: Master Data
  FIN70###: P&L reporting 
  FIN71###: Planning
  FIN72###: Balance Sheet 
  FIN74###: Profitability
  FIN77###: Group Reporting
  FIN80###: Cash Flow
•	Technical Layers CCC:
  0##: generic master data (for this application)
  1##: generic config tables / any other data you import (i.e. TVARV)
  2## - 8##: Logic
  9##: Buffer
  C##: Cubes 
  O##: OData
  E##: Extractor
  Q##: Query
