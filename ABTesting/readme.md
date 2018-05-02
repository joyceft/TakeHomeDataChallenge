# A/B Testing for Spanish Translation
## Project Description
Our client Company X is a worldwide e-commerce site with localized versions of the site. One of our DS noticed that Spain-based users have a muhch higher conversion rate than any other Spanish-speaking country. She wanted to know what's the reason by talking with international team of Spain and LatAm. The manager suggested that one reason could be translation. All Spanish-speaking countries had the same translation of the site which was written by a Spainiard. They agreed to try a test where each country would have its one translation written by a local. That is, Argentinian users would see a translation written by an Argentinian, Mexican users by a Mexican and so on. Obviously, nothing would change for users from Spain.

After they run the test however, the test is negative, which means that non-localized translation was doing better!

We want to know:
* Confirm that the test is actually negative. That is, it appears that the old version of the site with just one translation across Spain and LatAm performs better
* Explain why that might be happening. Are the localized translations really worse?
* If you identified what was wrong, design an algorithm that would return FALSE if the same problem is happening in the future and TRUE if everything is good and te results can be trusted.

### Dataset Description
There are two table: 
* user_table: some information about the user, including their id, sex, age, country
* test_table: general information about the test results, including the user_id, date(whey they came to the site for the first time since the test started); source(marketing channel: Ads, SEO, Direct); device; browser_language(chosen by user); ads_channel(if user came from Ads, then the site where ads was displayed was recorded); browser; conversion(0,1); test(users are randomly splited into 1-test, 0-control, for Spanish-based users, this is 0 since there is no change)
