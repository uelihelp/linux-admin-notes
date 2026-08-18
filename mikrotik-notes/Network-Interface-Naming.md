```text
  MMM      MMM       KKK                          TTTTTTTTTTT      KKK
  MMMM    MMMM       KKK                          TTTTTTTTTTT      KKK
  MMM MMMM MMM  III  KKK  KKK  RRRRRR     OOOOOO      TTT     III  KKK  KKK
  MMM  MM  MMM  III  KKKKK     RRR  RRR  OOO  OOO     TTT     III  KKKKK
  MMM      MMM  III  KKK KKK   RRRRRR    OOO  OOO     TTT     III  KKK KKK
  MMM      MMM  III  KKK  KKK  RRR  RRR   OOOOOO      TTT     III  KKK  KKK

  MikroTik RouterOS 7.20.8 (c) 1999-2026       https://www.mikrotik.com/
```

# Network Interface Naming

## Access Port

| Kürzel | Beschreibung | Format | Beispiel |

|---|---|---|---|

| `e` | Ethernet Access Port zu einem Subnetz | `e<SWPort>-<netname>` | `e99-netname` |

## To Host

| Kürzel | Beschreibung | Format | Beispiel |

|---|---|---|---|

| `e` | Ethernet-Verbindung zu einem Host | `e<SWPort>-<hostname>-<dstport>` | `e99-server01-1` |

| `s` | SFP+-Verbindung zu einem Host | `s<SWPort>-<hostname>-<dstport>` | `s99-server01-1` |

| `q1s1` | 1/4 QSFP+-Verbindung zu einem Host | `q1s1<SWPort>-<hostname>-<dstport>` | `q1s1-server01-1` |

## Bond (LACP Gruppe)

| Kürzel | Beschreibung | Format | Beispiel |

|---|---|---|---|

| `b` | LACP Bond aus mehreren Switch-Ports | `b<SWPort>-<hostname>` | `b99-server01` |

## VLAN

| Kürzel | Beschreibung | Format | Beispiel |

|---|---|---|---|

| `v` | VLAN-Zuordnung zu einem Subnetz | `v<VID>-<netname>` | `v99-netname` |

## Bridge

| Kürzel | Beschreibung | Format | Beispiel |

|---|---|---|---|

| `br` | Software-Bridge | `br-<name>` | `br-br0` |

  
> **Note:** Interface names do not contain spaces. Hyphens (\`-\`) are used as separators.

