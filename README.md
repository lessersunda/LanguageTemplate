# LanguageTemplate
Template for creating new word lists for inclusion in LexiRumah

## Step 0
Copy this entire folder (or download this repository as ZIP file and unpack it)
        into your favourite working directory and rename it to the name of the
        language you are working on.

**NOTE** *Please avoid renaming anything else. You may freely delete files that
          you have no use for.*

## Step 1
Put a description of the source in the folder "1 - description of the
        original source". You can choose whatever format is handy. Type a few
        lines in Word, save a webpage to that folder, copy the Excel sheet
        containing the metadata to here, whatever. Try to include as much
        metadata as possible with only a small amount of work.

## Step 2
Make a digital version of the original source available here. Scan a
        hard copy of the book and drop it inside "2 - original source", or run a
        web grabber or the source website, or store a backup of the FLEx corpus.
        If you can, create a link to a place where the original source is
        available online. If the original source is really well available
        elsewhere, or really huge, you may be able to justify skipping step 3.
        In that case, please place a text document in "2 - original source" that
        states your reasoning.

## Step 3
Formalize the source description. The folder "3 - normalized metadata of
        original source" contains examples for various types of sources, from
        fieldwork via published books to online databases. Take the one most
        fitting for your type of source, open it in a text editor (ideally eg.
        Notepad++; Word probably works, too) and modify it to reflect the
        source.

**NOTE** *If you are familiar with BibTeX, you may use any of it to describe the
          source. If you want to use non-standard fields or genres, get in
          contact.*

**NOTE** *If the source is published and has an entry on Glottolog (search via
          http://glottolog.org/langdoc/complexquery), just copy the
          BibTeX formatted citation from there.*

## Step 4
Take the language template (Pick Excel or CSV, delete the other) inside
        "4 - language metadata" and fill in name, location, description,
        Glottocode and Isocode of the language or lects described in your
        primary source as exactly as possible given the source and your
        background knowledge.

**NOTE** *If you have dialect information on a higher level of detail than in
          Glottolog, pick a Lect “ID” that is the next Glottocode above your
          variety, plus the first four, five or six letters of the glossonym,
          ie. the name of the variety as used in the source. (For field work
          data, this may also be the name of the village where the language is
          spoken.)*

**NOTE** *We can infer the region from the geo-coordinates, you may leave the
          “Region” column empty.*

**NOTE** *If you have done fieldwork and filled in a cultural questionnaire for
          our CultureRumah, put the name of your culture data file in the
          “Culture” column for the appropriate language(s). Otherwise leave that
          column empty.*

## Step 5
Create the word list (Pick one of Excel or CSV, delete the other). Take
        the word list template in "5 - wordlist created from original source"
        and fill it in. Make sure that every separate form is on a separate row
        in the word list, whether they express different concepts or are
        synonyms. This means that you can give comments for each individual
        form. You should choose whatever transcription the source uses for the
        “Form” column. If you have a choice, your “Form”s should be in a
        phonemic transcription which uniquely identifies the phonetic, segmented
        transcription in “Segments”.

**NOTE** *If the source lists forms that are obvious minor variants of each
          other, you are encouraged to pick one representative and add the
          variants in the “Comment” column.*

**NOTE** *Even if the source uses unconventional orthography for its
          pranscription, preserve it in the “Form” column.*

**NOTE** *Wherever the orthography for the “Form” column is very clean (the
          segmented phonetic realisation is obvious from the form), you may
          leave the “Segments” column empty. See "5 - wordlist created from
          original source/transcription.txt" for details.*

**NOTE** *If the transition from the sources' orthography to our standard broad
          phonetic transcription is following systematic orthography, you may
          leave “Segments” empty and instead provide a concise description of the
          orthographic profile (or of the phonetic realization of the phonemes,
          if the source transcribes phonemically). See "5 - wordlist created from
          original source/transcription.txt" for details.*

**NOTE** *If you leave the “Lect_ID” or “Concept_ID” fields empty, we assume you
          mean “The same value as in the row above”. So, if you have synonyms
          directly under each other, you may leave out their concept
          identifiers. And if you fill in a word list with only one language,
          put its “Lect_ID” (usually its Glottocode) in the first row. This
          means that if it is easy to work with the source in that way, the
          easiest way to include multiple word lists is to have them one above
          the other in the table.*

**NOTE** *You are allowed to reorder rows and columns as you wish. The importer
          is only interested in the “Concept_ID”, “Lect_ID”, “Form”, “Segments”
          and “Comment” columns and will IGNORE ALL OTHER COLUMNS. So if you
          notice an error in eg. the “Elicitation Notes”, you need to contact
          the editors or raise an issue on GitHub. Keep in mind that if you
          re-order rows, you need to have all “Concept_ID” and “Lect_ID” filled,
          otherwise you might mix up things.*

