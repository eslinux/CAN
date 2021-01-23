# CAN
CAN protocol

Encode and decode CAN frame:
https://github.com/reinzor/libcan-encode-decode/blob/master/include/can_encode_decode_inl.h

Note: Start position of signals: lsb start bit
      

=======================================

CAN Bus       | Bit Number

              | msb                 lsb

--------------+------------------------

Message ID    |

Control Field |

Data Byte 0   | 07 06 05 04 03 02 01 00

Data Byte 1   | 15 14 13 12 11 10 09 08

Data Byte 2   | 23 22 21 20 19 18 17 16

Data Byte 3   | 31 30 29 28 27 26 25 24

Data Byte 4   | 39 38 37 36 35 34 33 32

Data Byte 5   | 47 46 45 44 43 42 41 40

Data Byte 6   | 55 54 53 52 51 50 49 48

Data Byte 7   | 63 62 61 60 59 58 57 56

CRC Field     |

Ack. Field    |

End of Frame  |

=======================================




for example:
https://github.com/eerimoq/cantools/blob/master/tests/files/c_source/motohawk.c
