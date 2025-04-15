# CBT524
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 524 is from Ron Tatum and contains a subroutine to read   *   FILE 524
//*           a tape, and write from a tape, and do other functions *   FILE 524
//*           using EXCP.                                           *   FILE 524
//*                                                                 *   FILE 524
//*           email:  Ronald Tatum <rhtatum@door.net>               *   FILE 524
//*                                                                 *   FILE 524
//*   Short description of the routines:                            *   FILE 524
//*                                                                 *   FILE 524
//*   - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -   *   FILE 524
//*                                                                 *   FILE 524
//*      EXCP-LEVEL MAGNETIC TAPE READ/WRITE/CONTROL ROUTINES       *   FILE 524
//*                                                                 *   FILE 524
//*      SUBROUTINE ENTRY POINTS AND INPUT/OUTPUT PARAMETERS        *   FILE 524
//*                                                                 *   FILE 524
//*      CPRDOPEN - TO OPEN THE TAPE DATA SET                       *   FILE 524
//*       CPROPN IS AN ALTERNATE ENTRY POINT NAME FOR THIS          *   FILE 524
//*       OPERATION                                                 *   FILE 524
//*                                                                 *   FILE 524
//*        ANSWER (,DDNAME) INPUT TO ROUTINE. DDNAME DEFAULTS       *   FILE 524
//*         TO 'READIN  ' IF (,DDNAME) IS OMITTED.  IF              *   FILE 524
//*         SUPPLIED, IT MUST BE A CHAR STRING OF EIGHT BYTES,      *   FILE 524
//*         THE FIRST ALPHABETIC; MUST MATCH THE DDNAME FOR         *   FILE 524
//*         THE JCL STATEMENT FOR THE INPUT TAPE.                   *   FILE 524
//*                                                                 *   FILE 524
//*      CPRDCLS -  TO CLOSE THE DATA SET. NO PARMS.                *   FILE 524
//*       CPRCLS IS AN ALTERNATE ENTRY POINT NAME FOR CPRDCLS.      *   FILE 524
//*                                                                 *   FILE 524
//*      CPRD -     READ ONE PHYSICAL BLOCK. ANSWER, DATA, COUNT.   *   FILE 524
//*                                                                 *   FILE 524
//*      CPRDB -    READ BACKWARDS. ANSWER, DATA, COUNT.            *   FILE 524
//*                                                                 *   FILE 524
//*      CPSKRD -   READ A BLOCK, SKIPPING SOME BYTES AT FIRST.     *   FILE 524
//*                  ANSWER,DATA,COUNT.                             *   FILE 524
//*                                                                 *   FILE 524
//*      CPSKBR -   BACKWARD READ AFTER SKIP FROM END OF RECORD.    *   FILE 524
//*                  ANSWER, DATA, COUNT.                           *   FILE 524
//*                                                                 *   FILE 524
//*      CPFSF -    FORWARD SPACE ONE FILE. ANSWER.                 *   FILE 524
//*                                                                 *   FILE 524
//*      CPBSF -    BACKSPACE ONE FILE MARK. ANSWER.                *   FILE 524
//*                                                                 *   FILE 524
//*      CPFSB -    SKIP FORWARD ONE PHYSICAL BLOCK. ANSWER.        *   FILE 524
//*                                                                 *   FILE 524
//*      CPBSB -    BACKWARD SPACE ONE PHYSICAL BLOCK. ANSWER.      *   FILE 524
//*                                                                 *   FILE 524
//*      CPREW -    REWIND THE TAPE TO BOT. ANSWER.                 *   FILE 524
//*                                                                 *   FILE 524
//*      CPWTOPEN - OPEN THE OUTPUT TAPE DATA SET.                  *   FILE 524
//*       CPWOPN IS AN ALTERNATE ENTRY POINT NAME.                  *   FILE 524
//*                ANSWER (,DDNAME).                                *   FILE 524
//*                DDNAME DEFAULTS TO 'SYSTAPE ' IF OMITTED.        *   FILE 524
//*                                                                 *   FILE 524
//*      CPWT -    WRITE ONE PHYSICAL BLOCK. ANSWER, DATA, COUNT.   *   FILE 524
//*                                                                 *   FILE 524
//*      CPWTM -   WRITE A TAPE MARK. ANSWER.                       *   FILE 524
//*                                                                 *   FILE 524
//*      CPWERG -  ERASE GAP (NOMINALLY 3.5 INCHES). ANSWER.        *   FILE 524
//*                                                                 *   FILE 524
//*      CPERAS -  DATA SECURITY ERASE TO EOT MARKER. ANSWER.       *   FILE 524
//*                                                                 *   FILE 524
//*      CPWREW -  REWIND OUTPUT MAG TAPE VOLUME. ANSWER.           *   FILE 524
//*                                                                 *   FILE 524
//*      CPWRED -  READ ONE BLOCK FROM OUTPUT TAPE VOLUME.          *   FILE 524
//*                ANSWER, DATA,COUNT.                              *   FILE 524
//*                                                                 *   FILE 524
//*      CPWTCLS - CLOSE THE OUTPUT TAPE DATA SET.                  *   FILE 524
//*       CPWCLS IS AN ALTERNATE ENTRY POINT NAME. NO PARMS.        *   FILE 524
//*                                                                 *   FILE 524
```
