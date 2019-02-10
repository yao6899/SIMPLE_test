#include<stdio.h>
#include<string.h>
#define len 100
#define max_remind 100

int read_remind(char msg_str[],int n);

int main()
{
	char remind[max_remind][len+3];
	char day_str[3],msg_str[len+1];
	int remind_num=0;
	int i,j,day;
	
	for(;;){
		scanf("%d",&day);
		if(day==0)
			break;
		sprintf(day_str,"%2d",day);
		read_remind(msg_str,len);
		
		//printf("%d",i);
		
	for(i=0;i<remind_num;i++)
		if(strcmp(day_str,remind[i])<0)
			break;
	printf("%d\n",i);
	for(j=remind_num;j>i;j--)
		strcpy(remind[j],remind[j-1]);
	
	strcpy(remind[i],day_str);
	strcat(remind[i],msg_str);
	
	remind_num++;
	
	}
	
	//printf("\nDay Reminder\n");
	for(i=0;i<remind_num;i++)
		printf(" %s\n",remind[i]);
	
	return 0;
	
}
	
int read_remind(char msg_str[],int n){
	int input;
	int i=0;
	while((input=getchar())!='\n')
			if(i<n)
				msg_str[i++]=input;
	
	msg_str[i]='\0';
		
	return i;
}
	
