<!-- page_number: true -->

# ��3�� Pymee

---

# ���O�����m�F

+ Python�̃C���X�g�[��
+ �e�L�X�g�G�f�B�^�̃C���X�g�[��(vi, vim�ł���)
+ �׋������̃_�E�����[�h


# �Q���ɂ������Ă̒��ӎ���
+ ���pPC�͎������Ŏg�p���Ȃ��ŉ�����
+ zoom�z�M���s���܂��̂ł�����������
  + ���񂩂�^����s���܂�
+ �s���_�͋C�y�ɕ����ĉ������I

---

# �����̓��e

1. �O��̂����炢(for��/�t�@�C���ǂݍ���)
1. while��
1. �t�@�C����������
1. module

---
# ����̍u�`�ŗ��p����m��

����̍u�`�͑O��܂ł̍u�`�𓥂܂�����Ŏ��{���܂��B

+ for��
+ �t�@�C���ǂݍ���

---
# �O��̂����炢

�O��w�񂾃R�[�h�������炢���܂��傤�B

---

# for��
```python
#�usampleList�v�Ƃ������O�̃��X�g���쐬
sampleList = [1,2,3,4,5]

#for���ŁusampleList�v�̒��g��������o���ă��[�v
#�擪������o���Ė����܂Ń��[�v����B
for number in sampleList:
    print(number)
```
+ �o�͌���
```
1
2
3
4
5
```
---
+ omikuji�Ƃ������O�̑傫�Ȕ���0���珇�Ԃɔԍ��̕t����ꂽ�����Ȕ����i�[����Ă���C���[�W
![](./img/list.png)
---
# �����^
```python
# ����(omikuji)���쐬
# omikuji�Ƃ������O�̕ϐ��Ɏ����^��
# ��g���u���F�l�v�̌`�Ŋi�[���Ă���B
omikuji = {"��g":"���ׂĂ悵",
           "���g":"�܂��܂��悵",
           "���g":"�悵",
           "�g":"�������悵",
           "��":"��邵",
           }
print(omikuji["��g"])
```
+ �o�͌���
```
���ׂĂ悵
```
---
+ ���ꂼ��̒l���i�[���ꂽ�����J���錮���w�肷��C���[�W
![](./img/dic.png)
---
# �v���o���܂������H���̒m����O��ɁA�{���̍u�`���s���܂��B
---
# for���Ƃ́H

for���̓��X�g����l���擾���āA�擪����P���l�����o���Ȃ���J��Ԃ�(���[�v)�������������鎖���ł��܂��B

---
![](./img/for_flow.PNG)

---
�y�ᕶ(for��)�z
```python
#�usampleList�v�Ƃ������O�̃��X�g���쐬
sampleList = [1,2,3,4,5]

#for���ŁusampleList�v�̒��g��������o���ă��[�v
#�擪������o���Ė����܂Ń��[�v����B
for number in sampleList:
    print(number)
```
+ �o�͌���
```
1
2
3
4
5
```
---
�L�ڂ����ʂ�Afor���͎w�肵�����X�g�ɂ���l��S�ďo�͂��鎖���O��̍��ɂȂ��Ă��܂��B
�����X�g�ȊO�ɂ��^�v���A�����A������Ȃǂ����Âl�����o���܂��B

�ł����A�ȉ���Range�֐��𕹗p����ƃ��X�g�̏����Ȃ��Ŏw�肵���񐔂������[�v�ł��܂��B

�y�ᕶ(for��+Range�֐�)�z
```python
#range(����)��0�`(�L�ڂ�����)�̐�����������
#range�^�I�u�W�F�N�g(���X�g�̂悤�ȕ�)������B
#
#���L�̗ᕶ����0�`9(10��)�̒l��������
#range�^�I�u�W�F�N�g�������B
for number in range(10):

#�o�͎���+1����1�`10�ŏo�͂�����B
    print(number+1)
```
---
+ �o�͌���
```
1
2
3
4
5
6
7
8
9
10
```

��10�񃋁[�v���܂����A�o�͂�0����n�܂�̂ŏo�͂����l��0�`9�ɂȂ�܂��B���ׁ̈A�o�͎��̋L�ڂ�s+1�ɂ���1�`10��\�����Ă��܂��B
���l�����Ƃ��Ắu0���琔����10���ׂ����X�g���쐬�����v

---
## �T���v���v���O����������Ă݂܂��傤(for��)

�y���O�����z
�f�X�N�g�b�v(�ǂ��ł������ł�)�ɍ�ƃt�H���_���쐬���A�����ֈȉ��̖��O�Ńe�L�X�g�t�@�C�����쐬���ĉ������B�쐬�����t�@�C���ɃT���v���v���O�������L�ڂ��ĕۑ����ĉ������B
���S���R�s�y�Œ����Ă��܂���OK�ł��B

+ �t�@�C����

```
01_for.py
```
---

�y�T���v���v���O�����z

```python
#�uomikujiList�v�Ƃ������X�g���쐬
omikujiList = ['�d���^ �܂��܂��悵',
           '�����^ �悵',
           '���N�^ �������悵'
           ]

#for���ŁuomikujiList�v�̒��g��������o���ă��[�v
#�擪������o���Ė����܂Ń��[�v����B
for omikuji in omikujiList:
    print (omikuji);
```
---
�R�[�h����������ȉ��̃R�}���h�Ŏ��s���Ă݂܂��傤�B
+ ���s(windows�̏ꍇ)

```
py 01_for.py
```
+ ���s(���̑��̏ꍇ)

```
python3 01_for.py
```
+ �o�͌���
```
�d���^ �܂��܂��悵
�����^ �悵
���N�^ �������悵
```
---
# �t�@�C�����當�����ǂݍ���ł݂悤

�����python�𗘗p����̂ł���΁A�t�@�C�����o�͔͂����Ēʂ�Ȃ����ł��B
�܂��̓t�@�C�����當����ǂݍ���ł݂܂��傤�B
������uI/O�v�ƌ����P�ꂪ�o�Ă��܂����A�uINPUT/OUTPUT�v�̗��̂Łu����(�ǂݍ���)/�o��(�\��)�v���w���Ă��܂��B

---
![68%](./img/fileio_flow.PNG)

---
�y�ᕶ(�t�@�C��I/O)�z

```python
#�ǂݍ��ރt�@�C�����w��B
#���̏����ŋL�ڂ���ƈȉ��̒ʂ�ɒl���i�[�����B
#�@�E�t�@�C���ǂݍ��݌��F
#      inputSample.txt
#�@�E�t�@�C������ǂݍ��񂾒��g�̊i�[��F
#      inputAll(��s�����X�g�`���Ŋi�[�����)
inputAll = open("inputSample.txt", "r",encoding="utf-8")

#�t�@�C������ǂݍ��񂾒��g����s����for���ŏo�͂���B
for inputLine in inputAll:
    print (inputLine, end='');

#���₷���悤�ɍŌ�ɉ��s������
print('\n')

#�t�@�C����ǂݍ��񂾌�̓N���[�Y�������L�ڂ���B
#����������Ȃ��ƃ������ɃS�~���c��B(���삪�d���Ȃ��Ă���)
inputAll.close()
```
---
+ �o�͌���
```
�y��g�z
�Ґl�F�h�������҂ׂ�
�����F�����ɂ���
�����F�[���肷���
�]���F���������҂�
```

��L�̕��@�ŁA�\�[�X�R�[�h(.py�t�@�C��)��z�u�����t�H���_�Ɠ����t�H���_�ɔz�u���ꂽ�uinputSample.txt�v��ǂݍ��ގ����ł��܂��B

---
## �T���v���v���O����������Ă݂܂��傤(�t�@�C���ǂݍ���)
�y���O�����z
���O�����Ƃ��āA�ȉ��̓��e���L�ڂ����e�L�X�g�t�@�C������ƃt�H���_�ɕۑ����Ă����ĉ������B

+ �t�@�C����

```
inputSample.txt
```
+ �L�ړ��e

```
�y��g�z
�Ґl�F�h�������҂ׂ�
�����F�����ɂ���
�����F�[���肷���
�]���F���������҂�
```
---
���O���������t�@�C���Ƃ͕ʂɁA�ȉ��̃t�@�C�����쐬���ĉ������B

+ �t�@�C����

```
02_fileIO.py
```
�y�T���v���v���O�����z

```python
#�ǂݍ��ރt�@�C�����w��B
#�t�@�C���ǂݍ��݌��FinputSample.txt
inputAll = open("inputSample.txt", "r",encoding="utf-8")

for inputLine in inputAll:
    print (inputLine, end='');

print('\n')

inputAll.close()
```
---

+ ���s(windows�̏ꍇ)

```
py 02_fileIO.py
```
+ ���s(���̑��̏ꍇ)

```
python3 02_fileIO.py
```
+ �o�͌���
```
�y��g�z
�Ґl�F�h�������҂ׂ�
�����F�����ɂ���
�����F�[���肷���
�]���F���������҂�
```

�\�[�X�R�[�h�ɒ��ڋL�ڂ���Ă������e���e�L�X�g�t�@�C���ɂ܂Ƃ܂��������ŁA�啪���݂������ۂ��Ȃ��Ă����̂ł͂Ȃ��ł��傤���B

---
# ��O
���X�Ɩ����s���Ă���Ƒz��O�̎����N���肦�܂��B����Ȏ��̓t�H���[�����ĖႦ��Ə�����܂���ˁH
�v���O�������l�Ԃ��l���č�镨�ł�����A�z��O�̎���������񔭐����܂��B����Ȏ��Ƀt�H���[�����Ă�����d�g�݂��w�т܂��傤�B
���������A���������v���O�������Ԉ���Ă���ꍇ(�\���G���[)�͑ΏۊO�ł��B

---

![60%](./img/except_flow.PNG)

---


�y�ᕶ(��O)�z

<font style = "font-size: 97%">
   
```python
#�G���[�����������ۂɕʏ����֑J�ڂ��������ӏ���try�`except�ň͂ށB
#��{�I�ɑS���ł����B
try:

#�ᕶ�Ƃ��đ��݂��Ȃ��t�@�C�����w��
#�t�@�C�������Ԉ�����肵�đ��݂��Ȃ��t�@�C����
#�w�肷��ƃG���[�ɂȂ�܂��B
    inputAll = open("exception.txt", "r",encoding="utf-8")

    for inputLine in inputAll:
        print (inputLine, end='');

    print('\n')

    inputAll.close()

#��L��exception.txt�����݂��Ȃ��ׁA
#�G���[���������Ĉȉ���except�ƋL�ڂ��ꂽ�ӏ��̏��������s�����B
#
#�G���[���������Ȃ������ꍇ��except��ɋL�ڂ��ꂽ�R�[�h��
#���s����Ȃ��B
except:
    print("�G���[�I")
```
</font>

---

+ �o�͌���
```
�G���[�I
```

---

## �|�C���g
+ try�`except���L�ڂ��鎖�ŁA�����Ɏ��s�����ꍇ�̃t�H���[���ł���B
�@�˃G���[�����������ӏ��Ńv���O�����̎��s�����鎖��h����B

## �p�r
+ ���r���[�ɓ����Ă��܂����ۂ̌�n��
+ ���������G���[�̏ڍׂ����O�t�@�C���֋L��
etc...

---
## �T���v���v���O����������Ă݂܂��傤(��O)

+ �t�@�C����

```
03_except.py
```

---

�y�T���v���v���O�����z(1/2)
```python
#�G���[�������̏ڍ׎擾����
import sys

#�G���[�����������ۂɕʏ����֑J�ڂ��������ӏ���try�`except�ň͂ށB
try:

#�ᕶ�Ƃ��đ��݂��Ȃ��t�@�C�����w��
    inputAll = open("exception.txt", "r",encoding="utf-8")

    for inputLine in inputAll:
        print (inputLine, end='');

    print('\n')

```
---
�y�T���v���v���O�����z(2/2)
```python
#�t�@�C����������Ȃ����͈ȉ��̃R�[�h�����s�����B
#sys.exc_info()�ŃG���[�̏ڍׂ��m�F�ł���B
except FileNotFoundError:
    print("�t�@�C���ǂݍ��݃G���[�I")
    print(sys.exc_info())
#���̑��̃G���[�������͈ȉ��̃R�[�h�����s�����B
except:
    print("���̑��̃G���[�I")
    print(sys.exc_info())
#�G���[���������Ȃ������ꍇ�͈ȉ��̃R�[�h�����s�����B
else:
    print('����O�͔������܂���ł���')
#�ȉ��̃R�[�h�͂ǂ�ȏꍇ�ł����s�����B
finally:
    print('�����I��')
#�t�@�C�����I�[�v���ł��Ă���ꍇ�̂݃N���[�Y���������{����B
    if 'inputAll' in locals():
        inputAll.close()
```

---

+ ���s(windows�̏ꍇ)

```
py 03_except.py
```
+ ���s(���̑��̏ꍇ)

```
python3 03_except.py
```
+ �o�͌���
```
�t�@�C���ǂݍ��݃G���[�I
�����I��
Traceback (most recent call last):
�`

```
---
## 4��except��
+ except FileNotFoundError:
�@�ˑΏۃt�@�C�������݂��Ȃ����Ɏ��s�����
+ except:
�@�ˑS�ẴG���[�������Ɏ��s�����
+ else:
�@�ˑS�Đ���ɏ������ꂽ�ꍇ�Ɏ��s�����
+ finally:
�@�˂ǂ�ȏꍇ�ł����s�����

## �|�C���g
+ �ォ�珇�Ԃɏ��������
�@��except����ԏ�ɏ����Ƃ����ŏ�������Ă��܂��̂ŁA�ʃG���[�������ɏ���
+ sys.exc_info()�ŃG���[�̏ڍׂ��擾�ł���
�����O�Ɂuimport sys�v�̋L�q���K�v

---

# �܂Ƃ�(1/3)
1. �O��̂����炢(���X�g/�����^)

```python
omikuji = ['��g ���ׂĂ悵',
           '���g �܂��܂��悵',
           '���g �悵',
           '�g �������悵',
           '�� ��邵',
           ]
print(omikuji[0])
```
```python
omikuji = {"��g":"���ׂĂ悵",
           "���g":"�܂��܂��悵",
           "���g":"�悵",
           "�g":"�������悵",
           "��":"��邵",
           }
print(omikuji["��g"])
```

---

# �܂Ƃ�(2/3)
2. for��
```python
sampleList = [1,2,3,4,5]
for sample in sampleList:
    print(sample)
```
3. �t�@�C�����o��
```python
inputAll = open("inputSample.txt", "r",encoding="utf-8")
for inputLine in inputAll:
    print (inputLine, end='');
print('\n')
inputAll.close()
```

---

# �܂Ƃ�(3/3)
4. ��O
```python
try:
    inputAll = open("exception.txt", "r",encoding="utf-8")

    for inputLine in inputAll:
        print (inputLine, end='');
    print('\n')

except FileNotFoundError:
    print("�t�@�C���ǂݍ��݃G���[�I")
except:
    print("�G���[�I")
else:
    print('����O�͔������܂���ł���')
finally:
    print('�����I��')
    if 'inputAll' in locals():
        inputAll.close()
```
---
## �T���v���v���O����������Ă݂܂��傤(�܂Ƃ�)

�O�ł𓥂܂��A���̃R�[�h���쐬���ĉ������B

�y���O�����z
���O�����Ƃ��āA�ȉ��̓��e���L�ڂ����R�̃e�L�X�g�t�@�C������ƃt�H���_�ɕۑ����Ă����ĉ������B

�@
+ �t�@�C����

```
daikiti.txt
```
+ �L�ړ��e

```
�y��g�z
�Ґl�F�h�������҂ׂ�
�����F�����ɂ���
�����F�[���肷���
�]���F���������҂�
```

---

�A
+ �t�@�C����

```
kiti.txt
```
+ �L�ړ��e

```
�y�g�z
�Ґl�F�҂ĂΗ���
�����F�����炸
�����F�ǂ��o�����
�]���F�쓌���ǂ�
```
---

�B
+ �t�@�C����

```
kyo.txt
```
+ �L�ړ��e

```
�y���z
�Ґl�F���Ȃ�
�����F������
�����F�h�����
�]���F�R����
```
---
���O���������t�@�C���Ƃ͕ʂɁA�ȉ��̃t�@�C�����쐬���ĉ������B

+ �t�@�C����

```
04_summary.py
```
---

�y�T���v���v���O�����z(1/3)
```python
import sys
#�����_���Œl�����o���ׂ̏���
import random

#�G���[�����������ۂɕʏ����֑J�ڂ��������ӏ���try�`except�ň͂ށB
try:

#���݂����p�t�@�C����ǂݍ���
    daikiti = open("daikiti.txt", "r",encoding="utf-8")
    kiti    = open("kiti.txt", "r",encoding="utf-8")
    kyo     = open("kyo.txt", "r",encoding="utf-8")

#�ǂݍ��񂾂��݂����p�t�@�C���������^�ł܂Ƃ߂�
    inputOmikuji = {"��g":daikiti,
                    "�g":kiti,
                    "��":kyo}

#�����_���őI������ׂ̃L�[�ƂȂ�P������X�g�ŗp��
    omikujiList = inputOmikuji.keys()

#omikujiList�̒����烉���_���ň�I��
    randomOmikuji = random.choice(list(omikujiList))
```
---
�y�T���v���v���O�����z(2/3)
```python
#omikujiList���烉���_���ɑI�񂾉^��(������)���L�[�ɂ���inputOmikuji�ɃZ�b�g�����e�L�X�g�t�@�C���̒��g����I�񂾕�����ɑΉ�����t�@�C���̒��g��ǂݍ��ށB
    selectOmikuji = inputOmikuji[randomOmikuji]

#�ǂݍ��񂾃t�@�C���̒��g��1�s�����o���B
    for selectLine in selectOmikuji:
        print (selectLine, end='');

    print('\n')
```
---

�y�T���v���v���O�����z(3/3)
```python
#�t�@�C����������Ȃ����͈ȉ��̃R�[�h�����s�����B
except FileNotFoundError:
    print("�t�@�C���ǂݍ��݃G���[�I")
    print(sys.exc_info())
#���̑��̃G���[�������͈ȉ��̃R�[�h�����s�����B
except:
    print("���̑��̃G���[�I")
    print(sys.exc_info())
else:
    print('\n���݂����̌��ʂ͂ǂ��ł������H')
#�ȉ��̃R�[�h�͂ǂ�ȏꍇ�ł����s�����B
finally:
    if 'daikiti' in locals():
        daikiti.close()
    if 'kiti' in locals():
        kiti.close()
    if 'kyo' in locals():
        kyo.close()
```
---
+ ���s(windows�̏ꍇ)

```
py 04_summary.py
```
+ ���s(���̑��̏ꍇ)

```
python3 04_summary.py
```
---
+ �o�͌���
���ȉ��̂����ꂩ
```
�y��g�z
�Ґl�F�h�������҂ׂ�
�����F�����ɂ���
�����F�[���肷���
�]���F���������҂�
���݂����̌��ʂ͂ǂ��ł������H
```
```
�y�g�z
�Ґl�F�҂ĂΗ���
�����F�����炸
�����F�ǂ��o�����
�]���F�쓌���ǂ�
���݂����̌��ʂ͂ǂ��ł������H
```
```
�y���z
�Ґl�F���Ȃ�
�����F������
�����F�h�����
�]���F�R����
���݂����̌��ʂ͂ǂ��ł������H
```

---
# �݂Ȃ��񒷂��Ԃ����l�ł����I

---

# ����\��
+ �J��Ԃ�������Q�e
+ �t�@�C���̏�������

����͈̔͊O�̂��b
+ with open

---

# �A���P�[�g
+ ����̂��悢�����̂��߁A�A���P�[�g�ɂ����͂��������I

![400% center](./img/qr_3rd.png)

https://questant.jp/q/WP4SJ79K

---
# ���܂�
�I���C���[�́u�ދ��Ȃ��Ƃ�Python�ɂ�点�悤�v���A�s���{�������ݒn�N�C�Y�W�F�l���[�^�̃\�[�X�R�[�h�ł��B
�����̒m���{���œǂ߂܂��̂ŁA�u�`�����ł͕�����Ȃ��������͂ǂ����B
https://github.com/oreilly-japan/automatestuff-ja/blob/master/ch08/randomQuizGenerator.py

---
# ������ȂǁB�B�B
+ ���[�����O���X�g�ɂāA�^��A�s���_���C�y�ɕ����Ă��������I


