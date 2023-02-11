Install BLS signatures.

sudo git clone https://github.com/allforminers/bls.git

cd bls

unzip 20181101.zip

cd bls-signatures-20181101

cmake .

make -j8

sudo make install


NEW DASH COMpiled

sudo -s

apt-get update

apt-get install -y curl build-essential libtool autotools-dev automake pkg-config python3 bsdmainutils cmake

wget https://github.com/codablock/bls-signatures/archive/v20181101.zip

unzip v20181101.zip

cd bls-signatures-20181101

cmake .

make install

cd ..

git clone https://github.com/dashpay/dash

cd dash/depends

make -j30

cd ..

./autogen.sh

./configure --with-gui=no --prefix=$(pwd)/depends/x86_64-pc-linux-gnu

make -j8
