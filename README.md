<h2>Semantic Search with OpenAI Summarization</h2>
<p>This project extracts text from PDFs related to the Cambridge history of India and creates a dataframe with the extracted text. The dataframe is then saved as a CSV file.</p>
<h2>Libraries Used</h2>
<ul>
<li>os</li>
<li>glob</li>
<li>PyPDF2</li>
<li>pandas</li>
<li>numpy</li>
<li>sentence_transformers</li>
<li>chromadb</li>
<li>tqdm</li>
<li>re</li>
<li>torch</li>
<li>openai</li>
</ul>
<h2>Data</h2>
<p>17 PDF files related to the history of India</p>
<h2>Functions</h2>
<ul>
<li><code>filepathextractor()</code>: returns a list of file paths for a given file type</li>
<li><code>keep_unicode(text)</code>: keeps only Unicode characters in text</li>
<li><code>textdfcreator(filepaths)</code>: extracts text from PDFs and creates a dataframe with the extracted text</li>
</ul>
<h2>Process</h2>
<ol>
<li>PDFs related to the history of India are collected and stored as a list of file paths</li>
<li>The text is extracted from each PDF using the PdfReader function from the PyPDF2 library</li>
<li>The extracted text is cleaned using the <code>keep_unicode()</code> function and stored in a dataframe with the title and path of the PDF</li>
<li>The dataframe is then saved as a CSV file</li>
</ol>
<h2>Regular Expressions</h2>
<ul>
<li><code>sentence_end_re</code>: compiled regular expression to identify the end of a sentence</li>
<li><code>sentence_start_re</code>: compiled regular expression to identify the start of a sentence</li>
</ul>
<h2>Function</h2>
<ul>
<li><code>split_text(text)</code>: splits text into chunks of 190 words each.</li>
</ul>
<p><strong>Note:</strong> This code was tested on a set of 17 PDF files. The code to extract text from the PDFs is commented out because it is not necessary to re-run this step.</p>
