1����fork��һ����ĿA���Ҹ����˻��£���Ϊ��ĿB������ͬ���޸���һЩ��Ϣ������Ҫ���޸ĵ���Ϣͬ�������˻��µ���ĿB��

#�����ĿA��Զ�ֿ̲��ַ��upstream

git remote add upstream <��ĿA�Ĳֿ��ַ>

#����ĿA�ĸ����������ص�upstream��

git fetch upstream

#�л������Լ���Ҫmerge�ķ�֧���������þ�����master

git checkout master

#merge��ĿA�ĸ��µ����branch

git merge upstream/master


2�������git��ɾ��ָ�����ļ���Ŀ¼

#��ȡԶ�̵�Repo�����أ�����Ѿ��ڱ��أ������Թ��� 

git clone xxxxxx

#�ڱ��زֿ�ɾ���ļ� 

git rm �ҵ��ļ�

#�ڱ��زֿ�ɾ���ļ��� 

git rm -r �ҵ��ļ���/

#�˴�-r��ʾ�ݹ�������Ŀ¼�������Ҫɾ���ģ��ǿյ��ļ��У��˴����Բ��ô���-r��ǿ�Ƹ��¿��Դ���-f

#�ύ���� 

git commit -m"�ҵ��޸�"

#���͵�Զ�ֿ̲⣨����GitHub�� 

git push origin xxxxxx