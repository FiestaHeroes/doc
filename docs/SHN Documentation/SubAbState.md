| SubAbState              |              |                                                                               |
| ----------------------- | ------------ | ----------------------------------------------------------------------------- |
| SHINE_ABSTATE_ID        | ID           | When the SubAbState status abnormal ID is added, continue from the bottom ID. |
| STR[32]                 | InxName      | Interlocks with SubAbState of Sub State Abnormal Index AbState                |
| DWORD                   | Strength     | Specifies the status abnormality level                                        |
| INX["SubState"]         | Type         | abnormal status type                                                          |
| BYTE                    | SubType      |                                                                               |
| DWORD                   | KeepTime     | Specify status abnormality time                                               |
| INX["SubAbstateAction"] | ActionIndexA | Status Abnormality Attribute                                                  |
| DWORD                   | ActionArgA   | attribute value                                                               |
| INX["SubAbstateAction"] | ActionIndexB | Status Abnormality Attribute                                                  |
| DWORD                   | ActionArgB   | attribute value                                                               |
| INX["SubAbstateAction"] | ActionIndexC | Status Abnormality Attribute                                                  |
| DWORD                   | ActionArgC   | attribute value                                                               |
| INX["SubAbstateAction"] | ActionIndexD | Status Abnormality Attribute                                                  |
| DWORD                   | ActionArgD   | attribute value                                                               |

## Enums
```bash
typedef enum SubState {
    SUBAB_STRRATE=0,
    SUBAB_STRPLUS=1,
    SUBAB_WCPLUS=2,
    SUBAB_WCRATE=3,
    SUBAB_ACPLUS=4,
    SUBAB_ACRATE=5,
    SUBAB_DEXPLUS=6,
    SUBAB_TBPLUS=7,
    SUBAB_TBRATE=8,
    SUBAB_THPLUS=9,
    SUBAB_THRATE=10,
    SUBAB_INTPLUS=11,
    SUBAB_MAPLUS=12,
    SUBAB_MENPLUS=13,
    SUBAB_MRPLUS=14,
    SUBAB_MRRATE=15,
    SUBAB_DAMAGESHIELD=16,
    SUBAB_MANASHIELD=17,
    SUBAB_SHIELDACRATE=18,
    SUBAB_MOVESPEED=19,
    SUBAB_ATKSPEED=20,
    SUBAB_STUN=21,
    SUBAB_BLOODING=22,
    SUBAB_ENTANGLE=23,
    SUBAB_MAXHPRATE=24,
    SUBAB_MAXSPRATE=25,
    SUBAB_DEADHPSPRECOVRATE=26,
    SUBAB_DOTDAMAGE=27,
    SUBAB_FEAR=28,
    SUBAB_CONHEAL=29,
    SUBAB_CASTINGTIMEPLUS=30,
    SUBAB_COOLTIMEREMOVE=31,
    SUBAB_MAGICATTACKNOUSE=32,
    SUBAB_POISON=33,
    SUBAB_DISEASE=34,
    SUBAB_CURSE=35,
    SUBAB_RESIST=36,
    SUBAB_CRITICALRATE=37,
    SUBAB_DEFAULT=38,
    SUBAB_MAXHPPLUS=39,
    SUBAB_MAXSPPLUS=40,
    SUBAB_CONSPHEAL=41,
    SUBAB_QUESTSTUN=42,
    SUBAB_WCMINUS=43,
    SUBAB_DEXMINUS=44,
    SUBAB_ACMINUS=45,
    SUBAB_MRMINUS=46,
    SUBAB_STRMINUS=47,
    SUBAB_THMINUS=48,
    SUBAB_TBMINUS=49,
    SUBAB_CURSEMR=50,
    SUBAB_CURSETH=51,
    SUBAB_CURSEAC=52,
    SUBAB_CURSETB=53,
    SUBAB_CURSEDEX=54,
    SUBAB_CURSEWC=55,
    SUBAB_INTRATE=56,
    SUBAB_CURSECRITICAL=57,
    SUBAB_SELFREVIVE=58,
    SUBAB_RANGESHIELDCOUNTER=59,
    SUBAB_HIDE=60,
    SUBAB_BLIND=61,
    SUBAB_DEADLYBLESSING=62,
    SUBAB_GUILDBUFAC=63,
    SUBAB_NATURALENEMY=64,
    SUBAB_QUESTENTANGLE=65,
    SUBAB_CONHPSPHEAL=66,
    SUBAB_KNOCKBACK=67,
    SUBAB_FATALKNOCKBACK=68,
    SUBAB_EVENTTRANSFORM=69,
    SUBAB_CAPTIVATE=70,
    SUBAB_CANTHEAL=71,
    SUBAB_CANTCHAT=72,
    SUBAB_ACMODE=73,
    SUBAB_MRMODE=74,
    SUBAB_ANGRY=75,
    SUBAB_DAMAGENEGLECT=76,
    SUBAB_TIMEATTACK=77,
    SUBAB_DETACHPROCESS=78,
    SUBAB_HUMARWCRATE=79,
    SUBAB_HUMARACRATE=80,
    SUBAB_ACDOWNRATE=81,
    SUBAB_GTI=82,
    SUBAB_BURN=83,
    SUBAB_FITBLOODING=84,
    SUBAB_RANGEEVASION=85,
    SUBAB_USESPRATE=86,
    SUBAB_SOULFREE=87,
    SUBAB_ONETIMECANNOTUSESKILL=88,
    SUBAB_MOBAPU=89,
    SUBAB_HELGANONE=90,
    SUBAB_HELGBALL=91,
    SUBAB_UBAUP=92,
    SUBAB_UBADOWN=93,
    SUBAB_BURNPAINME=94,
    SUBAB_BURNPAINFOE=95,
    SUBAB_AIRBORNE=96,
    SUBAB_BOMBSHOT=97,
    SUBAB_CROSSDROP=98,
    SUBAB_METEOR=99,
    SUBAB_USESPDOWN=100,
    SUBAB_MENDOWNRATEME=101,
    SUBAB_MENDOWNRATE=102,
    SUBAB_CRIUPRATE=103,
    SUBAB_DMGSHIELD=104,
    SUBAB_CANNOTTARGET=105,
    SUBAB_HIDEDAMAGE=106,
    SUBAB_MAGICFIELD=107,
    SUBAB_MINEREWARD=108,
    SUBAB_EXPRATE=109,
    SUBAB_DROPRATE=110,
    SUBAB_MARATE=111,
    SUBAB_SURPRISE=112,
    SUBAB_DISPEL=113,
    SUBAB_RANGEDMGDOWNRATE=114,
    SUBAB_DMGSHIELDRATE=115,
    SUBAB_DMGDOWNRATE=116,
    SUBAB_MINHP=117,
    SUBAB_DELCASTING=118,
    SUBAB_RANGEDMGDOWNRATEATK=119,
    MAX_SUBSTATE=120
} SubState;
```
```bash
typedef enum SubAbstateAction {
    SAA_NONE=0,
    SAA_STRRATE=1,
    SAA_STRPLUS=2,
    SAA_WCPLUS=3,
    SAA_WCRATE=4,
    SAA_ACPLUS=5,
    SAA_ACRATE=6,
    SAA_DEXPLUS=7,
    SAA_TBPLUS=8,
    SAA_TBRATE=9,
    SAA_THPLUS=10,
    SAA_THRATE=11,
    SAA_INTPLUS=12,
    SAA_MAPLUS=13,
    SAA_MENTALPLUS=14,
    SAA_MRPLUS=15,
    SAA_MRRATE=16,
    SAA_SHIELDAMOUNT=17,
    SAA_SHIELDACRATE=18,
    SAA_NOMOVE=19,
    SAA_SPEEDRATE=20,
    SAA_ATTACKSPEEDRATE=21,
    SAA_MAXHPRATE=22,
    SAA_MAXSPRATE=23,
    SAA_DEADHPSPRECOVRATE=24,
    SAA_NOATTACK=25,
    SAA_TICK=26,
    SAA_DOTDAMAGE=27,
    SAA_CONHEAL=28,
    SAA_CASTINGTIMEPLUS=29,
    SAA_HEALAMOUNT=30,
    SAA_POISONRESISTRATE=31,
    SAA_DISEASERESISTRATE=32,
    SAA_CURSERESISTRATE=33,
    SAA_CRITICALRATE=34,
    SAA_MAXHPPLUS=35,
    SAA_MAXSPPLUS=36,
    SAA_INTRATE=37,
    SAA_FEAR=38,
    SAA_ALLSTATEPLUS=39,
    SAA_REVIVEHEALRATE=40,
    SAA_COUNT=41,
    SAA_SILIENCE=42,
    SAA_DEADLYBLESSING=43,
    SAA_DAMAGERATE=44,
    SAA_TARGETENEMY=45,
    SAA_MARATE=46,
    SAA_HEALRATE=47,
    SAA_DOTRATE=48,
    SAA_AWAY=49,
    SAA_TOTALDAMAGERATE=50,
    SAA_DISPELSPEEDRATE=51,
    SAA_SETABSTATEME=52,
    SAA_SETABSTATEFRIEND=53,
    SAA_SETABSTATE=54,
    SAA_AREA=55,
    SAA_GTIRESISTRATE=56,
    SAA_MAXHPRATEDAMAGE=57,
    SAA_METAABILITY=58,
    SAA_METASKIN=59,
    SAA_MISSRATE=60,
    SAA_REFLECTDAMAGE=61,
    SAA_RELESEACTION=62,
    SAA_SCANENEMYUSER=63,
    SAA_TARGETALL=64,
    SAA_HIDEENEMY=65,
    SAA_TARGETNOTME=66,
    SAA_DOTDIEDAMAGE=67,
    SAA_ADDALLDOTDMG=68,
    SAA_ADDBLOODINGDMG=69,
    SAA_ADDPOISONDMG=70,
    SAA_EVASIONAMOUNT=71,
    SAA_USESPRATE=72,
    SAA_ACMINUS=73,
    SAA_ACDOWNRATE=74,
    SAA_SUBTRACTALLDOTDMG=75,
    SAA_SUBTRACTBLOODINGDMG=76,
    SAA_SUBTRACTPOISONDMG=77,
    SAA_ATKSPEEDDOWNRATE=78,
    SAA_AWAYBACK=79,
    SAA_CRITICALDOWNRATE=80,
    SAA_DEXMINUS=81,
    SAA_HEALAMOUNTMINUS=82,
    SAA_MAMINUS=83,
    SAA_MADOWNRATE=84,
    SAA_MAXHPDOWNRATE=85,
    SAA_MRMINUS=86,
    SAA_MRDOWNRATE=87,
    SAA_SPEEDDOWNRATE=88,
    SAA_STRMINUS=89,
    SAA_TBMINUS=90,
    SAA_TBDOWNRATE=91,
    SAA_THMINUS=92,
    SAA_THDOWNRATE=93,
    SAA_WCMINUS=94,
    SAA_WCDOWNRATE=95,
    SAA_DOTWCRATE=96,
    SAA_TARGETNUMVER=97,
    SAA_DOTMARATE=98,
    SAA_MENDOWNRATE=99,
    SAA_USESPDOWN=100,
    SAA_CRIUPRATE=101,
    SAA_MRSHIELDRATE=102,
    SAA_ACSHIELDRATE=103,
    SAA_MONSTERSTICK=104,
    SAA_SETACTIVESKILL=105,
    SAA_HPRATEDAMAGE=106,
    SAA_EXPRATE=107,
    SAA_DROPRATE=108,
    SAA_AWAYBACKSPOT=109,
    SAA_STOPANI=110,
    SAA_DOTDMGDOWNRATE=111,
    SAA_SHIELDRATE=112,
    SAA_LPAMOUNT=113,
    SAA_MINHP=114,
    SAA_DMGDOWNRATE=115,
    SAA_SPEEDRESISTRATE=116,
    SAA_MELEE=117,
    SAA_RANGE=118,
    SAA_ALLSTATPLUS=119,
    SAA_RANGEOVER=120,
    MAX_SUBABSTATEACTION=121
} SubAbstateAction;
```