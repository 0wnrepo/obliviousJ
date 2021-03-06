Shape CPU (Java Implementation)
===============================

Introduction
============

A growing number of compute and data storage jobs is performed on remote resources. In a cloud environment the customer can’t be sure where a particular job is physically executed and thus cannot rely on the security and confidentiality of the remote resource. A solution for this problem is the operation on encrypted functions and encrypted data. This enables a customer to generate a program that can be executed by a third party, without revealing the underlying algorithm or the processed data. This helps securing applications and data in a distributed digital ecosystem. The shapeCPU is a method to compute a secret program on an untrusted resource using fully homomorphic encrypted circuits. The concept solves the problems of encrypted storage access with encrypted addresses and encrypted branching: in contrast to other approaches, like static one-pass circuit simulations, our system supports dynamic parameters and non-sequential programs, that render branch-decisions at runtime and cannot be represented in a circuit with hard-wired in-circuit parameters and data. 

Currently the runtime properties of the shapeCPU are very slow due to the underlying homomorphic cryptographic operations. We hope this open source project can serve as a foundation to actively encourage research and participation into optimizing both the cryptographic performance as well as the CPU performance. If you are interested in collaborating with us please drop us a line.

The Java implementation comprises the reference runtime environment for an encrypted program and an assembler skeleton to generate the encrypted machine code. However, the Java version does not encrypt but feel free to interface with libScarab via JNI. Find the encrypting C implementation of shapeCPU on github under hcrypt-project/oblivious.

References
==========

[1] M. Brenner, J. Wiebelitz, G. v. Voigt, M. Smith, Secret Program Execution in the Cloud applying Homomorphic Encryption, Proceedings of the 5th IEEE International Conference on Digital Ecosystems and Technologies (IEEE DEST 2011)

[2] M. Brenner, J. Wiebelitz, G. v. Voigt, M. Smith, A Smart-Gentry based Software System for Secret Program Execution, Proceedings of the 6th International Conference on Security and Cryptography (SECRYPT 2011)

[3] H. Perl, M. Brenner, M. Smith, POSTER: An Implementation of the Fully Homomorphic Smart-Vercauteren Crypto-System, Proceedings of the 18th ACM Conference on Computer and Communications Security (ACM CCS 2011)

[4] H. Perl, Y. Mohammed, M. Brenner, M. Smith, Fast Confidential Search for Bio-Medical Data Using Bloom Filters and Homomorphic Cryptography,Proceedings of the 8th IEEE International Conference on eScience (IEEE eScience 2012)

[5] M. Brenner, H. Perl, M. Smith, Practical Applications of Homomorphic Encryption,Proceedings of the 7th International Conference on Security and Cryptography (SECRYPT 2012)

[6] M. Brenner, H. Perl, M. Smith, How Practical is Homomorphically Encrypted Program Execution? An Implementation and Performance Evaluation,11th IEEE International Conference on Trust, Security and Privacy in Computing and Communications (IEEE TrustCom-2012)

[7] M. Brenner, M. Smith, POSTER: Caching Oblivious Memory Access under Fully Homomorphic Encryption, Proceedings of the 20th ACM Conference on Computer and Communications Security (ACM CCS 2013)

License
=======

Copyright © 2011

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

SOFTWARE AND SOURCE CODE MAY BE DOWNLOADED AND MODIFIED FOR EDUCATIONAL OR ACADEMIC USE. PATENT PCT/EP2678772B1.
