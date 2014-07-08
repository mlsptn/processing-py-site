# Processing Py Site

The directory structure for processing-py-site is as follows:

<pre>
+-processing-py-site/
  |
  +-Cover/
  |
  +-Examples/
  |
  +-Overview/
  |
  +-Reference/
  | |
  | +-api_en/
  |   |
  |   +-htmlconversions/
  |   |
  |   +-include/
  |
  +-Tutorials/
</pre>

The script Reference/api_en/htmlgenerator.py generates .html Reference pages from the .xml files in the same directory.

Run it using this line, which assumes you are in Reference/api_en:

for file in *.xml; do python htmlgenerator.py $file htmlconversions/${file%.*}_.html; done

