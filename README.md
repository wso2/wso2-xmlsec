# wso2-xmlsec
This is a fork of Apache santuario-xml-security-java repository. Forked @ tag level 1.5.6

# Patching instructions
After doing a code change build this repository with JDK 6 + maven 3.2.5 combination.
You can download JDK 6 from atuwa (internal)
We  are skipping tests in the default profile. So, to build with tests use the following command.
```
mvn clean install -P withtest
```

Test results when fork happens

`Results :

Tests in error:
C14N11Test.test_xmlid_1:56->test_c14n11:161 » XMLSignature javax.xml.crypto.UR...
C14N11Test.test_xmlid_2:61->test_c14n11:161 » XMLSignature javax.xml.crypto.UR...
C14N11Test.test_xmlspace_1:66->test_c14n11:161 » XMLSignature javax.xml.crypto...
C14N11Test.test_xmlspace_2:71->test_c14n11:161 » XMLSignature javax.xml.crypto...
C14N11Test.test_xmlspace_3:76->test_c14n11:161 » XMLSignature javax.xml.crypto...
C14N11Test.test_xmlspace_4:81->test_c14n11:161 » XMLSignature javax.xml.crypto...
C14N11Test.test_xmllang_1:86->test_c14n11:161 » XMLSignature javax.xml.crypto....
C14N11Test.test_xmllang_2:91->test_c14n11:161 » XMLSignature javax.xml.crypto....
C14N11Test.test_xmllang_3:96->test_c14n11:161 » XMLSignature javax.xml.crypto....
C14N11Test.test_xmllang_4:101->test_c14n11:161 » XMLSignature javax.xml.crypto...
C14N11Test.test_xmlbase_prop_1:106->test_c14n11:161 » XMLSignature javax.xml.c...
C14N11Test.test_xmlbase_prop_2:111->test_c14n11:161 » XMLSignature javax.xml.c...
C14N11Test.test_xmlbase_prop_3:116->test_c14n11:161 » XMLSignature javax.xml.c...
C14N11Test.test_xmlbase_prop_4:121->test_c14n11:161 » XMLSignature javax.xml.c...
C14N11Test.test_xmlbase_prop_5:126->test_c14n11:161 » XMLSignature javax.xml.c...
C14N11Test.test_xmlbase_prop_6:131->test_c14n11:161 » XMLSignature javax.xml.c...
C14N11Test.test_xmlbase_prop_7:136->test_c14n11:161 » XMLSignature javax.xml.c...
ValidateSignatureTest.test_signature_external_c14n_xmlattrs:82 » XMLSignature ...
BaltimoreIaik2Test.testSignature:58 » XMLSignature javax.xml.crypto.URIReferen...
InteropC14nTest.test_y3_signature:78 » XMLSignature javax.xml.crypto.URIRefere...
IaikTransformsTest.test_base64DecodeSignature:57 » XMLSignature javax.xml.cryp...
IaikTransformsTest.test_c14nSignature:76 » XMLSignature javax.xml.crypto.URIRe...
CreateBaltimore23Test.test_create_signature_retrievalmethod_rawx509crt:220->test_create_signature_external:650 » XMLSignature
BaltimoreEncTest.test_five_content_aes256_cbc:186->decryptElement:410 » XMLEncryption
BaltimoreEncTest.test_five_content_aes128_cbc_kw_aes192:208->decryptElement:408->findKey:533 » XMLEncryption
BaltimoreEncTest.test_five_element_aes192_cbc_ref:275->decryptElement:410 » XMLEncryption
BaltimoreEncTest.test_five_data_aes256_cbc_3des:321->decryptData:451 » XMLEncryption
BaltimoreEncTest.test_five_data_aes192_cbc_aes256:343->decryptData:448->findKey:533 » XMLEncryption
XMLCipherTest.testAES128ElementAES192KWCipherUsingKEK:144 » XMLEncryption Ille...
XMLCipherTest.testAES128ElementRSAKWCipherUsingKEK:227 » XMLEncryption Illegal...
XMLCipherTest.testAES192ElementAES256KWCipher:298 » XMLEncryption Illegal key ...
XMLCipherTest.testAes192ElementCipher:450 » XMLEncryption Illegal key size or ...
XMLCipherTest.testAes265ElementCipher:496 » XMLEncryption Illegal key size or ...

Tests run: 498, Failures: 0, Errors: 33, Skipped: 12
`
