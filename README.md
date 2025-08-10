# Test1
test

			SELECT distinct  D.SrcCDCustomerID, a.DateTaken  from  SRG_SrcCDDebt a
JOIN (SELECT  b.SRCCDCUstomerID,a.SRCMasterID from SRG_SrcCDCustomer a
JOin SRG_SrcCDCustomer b on a.CustomerID = b.CustomerID AND a.AdviceID = b.AdviceID AND a.SRCMasterID = 148
Where a.SrcCDCustomerID in (SELECT SRCCDCUstomerID from SRG_SrcCDCustomer where SRCMasterID = 148) and b.SRCMasterID = 149) d
ON a.SrcMasterID=d.SRCMasterID WHERE A.SRCMasterID = 148
