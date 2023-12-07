**What is your security recommendation? Why did you choose it?**

Implementation of encrypted local storage is recommended.

A common misconception is that offline apps are less vulnerable to
security threats. However, the absence of internet connectivity does not
eliminate risks such as device loss and unauthorized physical access.
The Expenses app store user's personal financial information. Although
the app does not require an internet connection to operate, it uses its
local data storage to store all data. If the physical device is lost
and/or stolen and then accessed by any third party, the user's data will
be leaked which leads to a data breach situation. The reputation of the
developer will potentially be damaged.

Encryption ensures that data stored on local storage is not in a
readable format without the correct decryption key. Data remains
incomprehensible and secure if any third party gains physical access to
the local data storage.

In this case, our developed expenses tracker app, SQLCipher is
recommended. According to \[1\], SQLCipher is a security extension to
the SQLite database platform that facilitates the creation of encrypted
databases. It uses the internal SQLite Codec API to insert a callback
into the pager system that can operate on database pages immediately
before they are written to and read from storage. With SQLCipher, the
entire database file, including data, tables, indexes, etc. is
encrypted.

**Who does the recommendation benefit (end-user, developer, etc.)?**

For end users, encrypting data ensures that it remains confidential. In
the event of a lost and/or compromised device, the encrypted data
remains secure and inaccessible to unauthorized parties.

For developers, implementing security measures by using data encryption
enhances the app's credibility which increases of user's trust. Since
data breach leads to severe consequences such as legal ramifications and
financial penalty, by encrypting data, developers do not merely protect
their users but also the sustainability of their app.

**If the recommendation was found somewhere other than the provided
checklist, include a link to it.**

The recommendation was found in the provided checklist.

**When would the recommendation have to be implemented (based on how
serious the security risk is)?**

Encryption should be implemented during the initial stage of the app
development. It helps to ensure that all financial data is protected
from first use. Before the launch of the app, other than developing data
encryption, testing is crucial to ensure that any data collected during
the testing phases is also secure. In addition, bug(s) can be fixed
before the app is released to the public.

**Why do you think your project needs your recommendation?**

The app that we developed is an expenses tracker app that collects and
stores user's financial data which is sensitive data. Loss of encryption
data implemented exposes the user's data at risk if the user loses
his/her physical device and/or if his/her physical device is accessed by
third parties without authorization.

**How do you think your recommendation could be applied?**

For Android apps, SQLCipher can be integrated seamlessly with SQLite.
Since we developed this expense tracker app for Android, using SQLCipher
for data encryption is an excellent choice.

**How feasible would the implementation be?**

The implementation of SQLCipher for data encryption in our app is
feasible. The technical requirements are straightforward while the
impact on development time is moderate, primarily for integration and
testing phases. Compared with the enhanced data protection resulted, the
impact is minimal. From the user's perspective, the implementation of
data encryption is transparent, and the app's functionality remains
unaltered.

**Reference**

\[1\] Zetetic, LLC. "SQLCipher Design." Zetetic LCC. Accessed: December
5, 2023. \[Online.\] Available:
https://www.zetetic.net/sqlcipher/design/.
