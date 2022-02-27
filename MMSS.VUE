/* MEMBER SPOUSE JOINED TABLE */

DROP VIEW BUNNELL.MMSS;

CREATE VIEW BUNNELL.MMSS
       (MEMBF,
        MFN,
        MMN,
        MLN,
        MDBY,
        MDBM,
        MPB,
        MBTN,
        MDDY,
        MDDM,
        MPD,
        MDTN,
        MG,
        MBY,
        MBM,
        MCB,
        PF,
        PSP,
        GEN,
        SP,
        SFN,
        SMN,
        SLN,
        SDBY,
        SDBM,
        SPB,
        SBTN,
        SDMY,
        SDMM,
        SPM,
        SMTN,
        SCM,
        SDDY,
        SDDM,
        SPD,
        SDTN,
        SG)

AS     (SELECT

        MEMBER.MEMBF,
        MEMBER.MFN,
        MEMBER.MMN,
        MEMBER.MLN,
        MEMBER.MDBY,
        MEMBER.MDBM,
        MEMBER.MPB,
        MEMBER.MBTN,
        MEMBER.MDDY,
        MEMBER.MDDM,
        MEMBER.MPD,
        MEMBER.MDTN,
        MEMBER.MG,
        MEMBER.MBY,
        MEMBER.MBM,
        MEMBER.MCB,
        MEMBER.PF,
        MEMBER.PSP,
        MEMBER.GEN,
        SPOUSE.SP,
        SPOUSE.SFN,
        SPOUSE.SMN,
        SPOUSE.SLN,
        SPOUSE.SDBY,
        SPOUSE.SDBM,
        SPOUSE.SPB,
        SPOUSE.SBTN,
        SPOUSE.SDMY,
        SPOUSE.SDMM,
        SPOUSE.SPM,
        SPOUSE.SMTN,
        SPOUSE.SCM,
        SPOUSE.SDDY,
        SPOUSE.SDDM,
        SPOUSE.SPD,
        SPOUSE.SDTN,
        SPOUSE.SG

        FROM BUNNELL.MM MEMBER LEFT OUTER JOIN BUNNELL.SS SPOUSE
             ON MEMBER.MEMBF = SPOUSE.MEMBF);




