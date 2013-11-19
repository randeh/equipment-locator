equipment-locator
=================

Locate circuits in racks with known layout. Must be lightweight and available offline.

Layout
------

There is one circuit per customer (also referred to as equipment number), circuits are numbered consecutively from 0. There are 8 circuits per card and 8 cards per LCT, organised as so:

    +-------------------------------------------+
    | +--+ +--+ +--+ +--+   +--+ +--+ +--+ +--+ |
    | |14| |15| |30| |31|   |46| |47| |62| |63| |
    | |12| |13| |28| |29|   |44| |45| |60| |61| |
    | |10| |11| |26| |27| L |42| |43| |58| |59| |
    | | 8| | 9| |24| |25| C |40| |41| |56| |57| |
    | | 6| | 7| |22| |23| T |38| |39| |54| |55| |
    | | 4| | 5| |20| |21| 0 |36| |37| |52| |53| |
    | | 2| | 3| |18| |19|   |34| |35| |50| |51| |
    | | 0| | 1| |16| |17|   |32| |33| |48| |49| |
    | +--+ +--+ +--+ +--+   +--+ +--+ +--+ +--+ |
    +-------------------------------------------+

where columns represent cards. Cards are numbered 1-8 from left to right within each LCT, whilst rows of circuits are numbered 1-8 from bottom to top. There can be up to 32 LCTs (totalling 2048 circuits) within a concentrator (CONC), and they are numbered 0-31.
