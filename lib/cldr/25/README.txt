This was generated by:

svn co http://unicode.org/repos/cldr/tags/release-25 cldr
cd cldr
patch -p0 <$GWT_TOOLS/lib/cldr/25/GoogleMods.patch
cd tools/java
ant jar
cp cldr.jar $GWT_TOOLS/lib/cldr/25

cp $GWT_TOOLS/lib/icu4j/53.1/icu4j.jar     $GWT_TOOLS/lib/cldr/25
cp $GWT_TOOLS/lib/icu4j/53.1/utilities.jar $GWT_TOOLS/lib/cldr/25
