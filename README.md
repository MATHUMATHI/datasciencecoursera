private static Set supportedExts; 
public Set getSupportedExtensions() {
if (supportedExts == null) {
supportedExts = new HashSet();
supportedExts.add(PKIXExtensions.KeyUsage_Id.toString());
supportedExts.add(PKIXExtensions.ExtendedKeyUsage_Id.toString());
supportedExts.add(PKIXExtensions.SubjectAlternativeName_Id.toString());
supportedExts = Collections.unmodifiableSet(supportedExts);
}
return supportedExts;
}
