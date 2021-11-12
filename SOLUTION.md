cd /
mkdir /tmp/"Coordinates-Location"
mkdir /tmp/"Coordinates-Location"/North
cd tmp/"Coordinates-Location"/North
echo "9°" > NDegree.txt
echo "5'" > NMinutes.txt
echo '38.1"' > NSeconds.txt
cat N* > NorthCoordinate.txt
cd /tmp/"Coordinates-Location"
mv North/NorthCoordinate.txt North.txt
mkdir /tmp/"Coordinates-Location"/East
cd East
echo "76°" > EDegree.txt
echo "29'" > EMinutes.txt
echo '30.8"' > ESeconds.txt
cat E* > EastCoordinate.txt
cd /tmp/"Coordinates-Location"
mv East/EastCoordinate.txt East.txt
cat North.txt East.txt > Location-Coordinate.txt
