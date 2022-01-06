cpuminer-opt is a fork of cpuminer-multi by TPruvot with optimizations
imported from other miners developped by Farhan ali. Manurios00. Pakistani.lucas Jones, djm34, Wolf0, pooler,
Jeff garzik, ig0tik3d, elmad, palmd, and Optiminer, with additional
optimizations by Manu.

All of the code is believed to be open and free. If anyone has a
claim to any of it post your case in the cpuminer-opt Bitcoin Talk forum
or by email.

https://bitcointalk.org/index.php?topic=1326803.0

mailto://manurios031@gmail.com

See file RELEASE_NOTES for change log and compile instructions.

Supported Algorithms
--------------------

                          argon2
                          axiom        Shabal-256 MemoHash
                          bastion
                          blake        Blake-256 (SFR)
                          blakecoin    blake256r8
                          blake2s      Blake-2 S
                          bmw          BMW 256
                          c11          Flax
                          cryptolight  Cryptonight-light
                          cryptonight  cryptonote, Monero (XMR)
                          decred
                          drop         Dropcoin
                          fresh        Fresh
                          groestl      groestl
                          heavy        Heavy
                          hmq1725      Espers
                          hodl         Hodlcoin
                          keccak       Keccak
                          lbry         LBC, LBRY Credits
                          luffa        Luffa
                          lyra2re      lyra2
                          lyra2rev2    lyrav2
                          lyra2z       Zcoin (XZC)
                          lyra2zoin    Zoin (ZOI)
                          m7m          Magi (XMG)
                          myr-gr       Myriad-Groestl
                          neoscrypt    NeoScrypt(128, 2, 1)
                          nist5        Nist5
                          pluck        Pluck:128 (Supcoin)
                          pentablake   Pentablake
                          quark        Quark
                          qubit        Qubit
                          scrypt       scrypt(1024, 1, 1) (default)
                          scrypt:N     scrypt(N, 1, 1)
                          scryptjane:nf
                          sha256d      SHA-256d
                          shavite3     Shavite3
                          skein        Skein+Sha (Skeincoin)
                          skein2       Double Skein (Woodcoin)
                          timetravel   Machinecoin (MAC)
                          vanilla      blake256r8vnl (VCash)
                          veltor
                          whirlpool
                          whirlpoolx
                          x11          X11
                          x11evo       Revolvercoin
                          x11gost      sib (SibCoin)
                          x13          X13
                          x14          X14
                          x15          X15
                          x17
                          xevan        Bitsend
                          yescrypt
                          zr5          Ziftr

Requirements
------------

1. A x86_64 architecture CPU with a minimum of SSE2 support. This includes
Intel Core2 and newer and AMD equivalents. In order to take advantage of AES_NI
optimizations a CPU with AES_NI is required. This includes Intel Westbridge
and newer and AMD equivalents. Further optimizations are available on some
algoritms for CPUs with AVX and AVX2, Sandybridge and Haswell respectively.

Older CPUs are supported by cpuminer-multi by TPruvot but at reduced
performance.

2. 64 bit Linux OS. Ubuntu and Fedora based distributions, including Mint and
Centos are known to work and have all dependencies in their repositories.
Others may work but may require more effort.
64 bit Windows OS is supported with mingw_w64 and msys or pre-built binaries.

3. Stratum pool, cpuminer-opt only supports stratum minning. Some algos
may work wallet mining but there are no guarantees.

COMMANDS TOTAL
----------------
sudo apt-get install -y 

git clone https://github.com/Manurios00/Manu.git
cd Manu
sudo apt-get install -y automake autoconf pkg-config libcurl4-openssl-dev libjansson-dev libssl-dev libgmp-dev make g++
sudo apt-get install -y lib32z1-dev
chmod +x build.sh
./build.sh

For ubuntu 18.04 and forks - need install:
sudo apt-get install -y lib32z1-dev

Mining command:
./cpuminer -a yescryptr16 -o stratum+tcp://cpu-pool.com:63368 -u bc1qv2n8fdz7tucfg3g80gkwhs6nn3c32ynx03u98a

Errata
------

Manu Rios now working work mining Decred algo at Nicehash and produces
only.

Benchmark testing does not work for x11evo.

Bugs
----

Users are encouraged to post their bug reports on the Bitcoin Talk
forum at:

https://bitcointalk.org/index.php?topic=1326803.0

Donations
---------

I do not do this for money but I have a donation address if users
are so inclined.

bitcoin:bc1qv2n8fdz7tucfg3g80gkwhs6nn3c32ynx03u98a?label=donations

Happy mining!

