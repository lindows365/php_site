����0.1



����0.2

ֱ���ύ
no changes added to commit (use "git add" and/or "git commit -a")
1.�鿴״̬
git status 
2.�����ļ�
git add ***.md
3.�ύ�ļ�
git commit -m '****'   ��-a����ȫ���ύ�������޸�״̬
4.push��master��
git push origin master  �ӱ���push��master��֧

5.�ļ��ıȽ�
git diff 

6.�Ƴ��ļ�
Ȼ�������� git rm ��¼�˴��Ƴ��ļ��Ĳ�����

����һ������ǣ���������ļ��� Git �ֿ���ɾ�����༴���ݴ������Ƴ���������Ȼϣ�������ڵ�ǰ����Ŀ¼�С����仰˵�����ǴӸ����嵥��ɾ��������һЩ������־�ļ�����һ��.a �����ļ�����С������ֿ��Ҫ�Ƴ����ٵ���ɾ���ļ����Ա��Ժ��� .gitignore �ļ��в��ϣ��� --cached ѡ��ɣ�
git rm --cached readme.txt



7.�ع���ʷ��־
git log 


8.��ԭ�ղŵ��޸�
(use "git checkout -- <file>..." to discard changes in working directory

git checkout  -- file.txt

9.�鿴Զ�� �����
 git remote -v
 
10.���Զ�ֿ̲�
git remote add pb https://github.com/lindows365/php_site.git
git remote show origin//��ʾԶ�� �ն˵�����

git remote rename pb paul  //����

git remote rm paul         //ɾ������


11.���ǩ
git tag v0.1


12.�����·�֧ �C git branch
git branch amazing_new_feature


13.�л���֧ �C git checkout

����ʹ��git branch�����Բ鿴��֧״̬��

14.�ϲ���֧ �C git merge

���ǵ� amazing_new_feature ��֧������������һ��featuer.txt����������������ӵ��ݴ������ύ��

Shell

$ git add feature.txt
$ git commit -m "New feature complete."
1
2
$ git add feature.txt
$ git commit -m "New feature complete."
�·�֧��������ˣ��ص�master��֧

Shell

$ git checkout master
1
$ git checkout master
����ȥ�鿴�ļ�����ᷢ�֣�֮ǰ������feature.txt�ļ������ˣ���Ϊmaster��֧�ϲ�û��feature.txt��ʹ��git merge �� amazing_new_feature ��֧�ϲ���master�ϡ�

Shell

$ git merge amazing_new_feature
1
$ git merge amazing_new_feature
ok! Ȼ���ٰ�amazing_new_feature ��֧ɾ���ɡ�

Shell

$ git branch -d amazing_new_feature
1
$ git branch -d amazing_new_feature

����һ��
error: src refspec remote does not match any.
�������취
git push origin HEAD:master
git push origin master --force 








