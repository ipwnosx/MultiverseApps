# groupsign ios apps


#! / bin / sh

# The name of the folder that is created on the desktop
myFolder = "groups"
# System name variable
UsersMac = "nawafmansour"
# Create a folder on your desktop
mkdir / Users / $ UsersMac / Desktop / $ myFolder
# The name of the folder in which all programs are extracted after the integration with the group extensions is completed
pathGroups = "Groups"
FoldersignAllGroups = "othmanresignAllGroups"
# Variable name tool Othman al-Mutairi
othmanResign = "othmanresign_source.sh"
# Desktop path
pathUser = "/ Users / $ UsersMac / Desktop / $ myFolder"

pathFolderGroups = "/ Users / $ UsersMac / Desktop / $ nameFolder /"
# Variable path for your office automatic folder creation process


mkdir / Users / $ UsersMac / Desktop / $ myFolder / $ pathGroups



for index in 1 2 3 4 5 6 7
do
mkdir / Users / $ UsersMac / Desktop / $ myFolder / "pro" $ index
done

for index in 1 2 3 4 5 6 7
do
rm -rf / Users / $ UsersMac / Desktop / $ FoldersignAllGroups / "pro" $ index / in / * ipa
done

for index in 1 2 3 4 5 6 7
do
rm -rf / Users / $ UsersMac / Desktop / $ FoldersignAllGroups / "pro" $ index / out / * ipa
done


for index in 1 2 3 4 5 6 7
do
cp -R / Users / $ UsersMac / Desktop / $ FoldersignAllGroups / in / * ipa / Users / $ UsersMac / Desktop / $ FoldersignAllGroups / "pro" $ index / in /
done

/ Users / $ UsersMac / Desktop / $ FoldersignAllGroups / pro1 / $ othmanResign "iPhone Distribution: NWAF MANSOUR (XXXXXXXXXXXXX)"
/ Users / $ UsersMac / Desktop / $ FoldersignAllGroups / pro2 / $ othmanResign "iPhone Distribution: NWAF MANSOUR (XXXXXXXXXXXXX)"
/ Users / $ UsersMac / Desktop / $ FoldersignAllGroups / pro3 / $ othmanResign "iPhone Distribution: NWAF MANSOUR (XXXXXXXXXXXXX)"
/ Users / $ UsersMac / Desktop / $ FoldersignAllGroups / pro4 / $ othmanResign "iPhone Distribution: NWAF MANSOUR (XXXXXXXXXXXXX)"
/ Users / $ UsersMac / Desktop / $ FoldersignAllGroups / pro5 / $ othmanResign "iPhone Distribution: NWAF MANSOUR (XXXXXXXXXXXXX)"
/ Users / $ UsersMac / Desktop / $ FoldersignAllGroups / pro6 / $ othmanResign "iPhone Distribution: NWAF MANSOUR (XXXXXXXXXXXXX)"
/ Users / $ UsersMac / Desktop / $ FoldersignAllGroups / pro7 / $ othmanResign "iPhone Distribution: NWAF MANSOUR (XXXXXXXXXXXXX)"



for index in 1 2 3 4 5 6 7
do
mv / Users / $ UsersMac / Desktop / $ FoldersignAllGroups / "pro" $ index / out / * ipa / Users / $ UsersMac / Desktop / $ myFolder / "pro" $ index
done

for index in 1 2 3 4 5 6 7
do
rm -rf / Users / $ UsersMac / Desktop / $ FoldersignAllGroups / "pro" $ index / in / * ipa
done


echo "======================== Software integration completed =================="
echo "======================== Wait 5 seconds to continue the rest of the orders ================ == "
# Wait five seconds
sleep 2s


# ===================== Renaming orders ==============
# Variable for desktop path
pathDeskTop = "/ Users / $ UsersMac / Desktop"
# Path folders on your desktop

NameFolder1 = "$ myFolder / pro1"
NameFolder2 = "$ myFolder / pro2"
NameFolder3 = "$ myFolder / pro3"
NameFolder4 = "$ myFolder / pro4"
NameFolder5 = "$ myFolder / pro5"
NameFolder6 = "$ myFolder / pro6"
NameFolder7 = "$ myFolder / pro7"

# The names you want to add at the end of the names of programs


nameIpa56 = "_ pro1"
nameIpa57 = "_ pro2"
nameIpa58 = "_ pro3"
nameIpa60 = "_ pro4"
nameIpa61 = "_ pro5"
nameIpa64 = "_ pro6"
nameIpa65 = "_ pro7"



# ======= Looks for programs in the format ipa and adds at the end the name you want ============
find $ pathDeskTop / $ NameFolder1 -name "* .ipa" -print | while read FILE
do mv "$ {FILE}" "` dirname $ {FILE} `/` basename $ {FILE} .ipa` $ nameIpa1.ipa "
done

find $ pathDeskTop / $ NameFolder2 -name "* .ipa" -print | while read FILE
do mv "$ {FILE}" "` dirname $ {FILE} `/` basename $ {FILE} .ipa` $ nameIpa2.ipa "
done


find $ pathDeskTop / $ NameFolder3 -name "* .ipa" -print | while read FILE
do mv "$ {FILE}" "` dirname $ {FILE} `/` basename $ {FILE} .ipa` $ nameIpa3.ipa "
done

find $ pathDeskTop / $ NameFolder4 -name "* .ipa" -print | while read FILE
do mv "$ {FILE}" "` dirname $ {FILE} `/` basename $ {FILE} .ipa` $ nameIpa4.ipa "
done

find $ pathDeskTop / $ NameFolder5 -name "* .ipa" -print | while read FILE
do mv "$ {FILE}" "` dirname $ {FILE} `/` basename $ {FILE} .ipa` $ nameIpa5.ipa "
done

find $ pathDeskTop / $ NameFolder6 -name "* .ipa" -print | while read FILE
do mv "$ {FILE}" "` dirname $ {FILE} `/` basename $ {FILE} .ipa` $ nameIpa6.ipa "
done

find $ pathDeskTop / $ NameFolder7 -name "* .ipa" -print | while read FILE
do mv "$ {FILE}" "` dirname $ {FILE} `/` basename $ {FILE} .ipa` $ nameIpa7.ipa "
done
