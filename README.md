int lengthOfLastWord(char* s) {
    int i,l,c=0;
    l=strlen(s);
    m:
    if(s[l-1]==' ')
    {
        l=l-1;
        goto m;
    }
    else{
    for(i=l-1;i>=0;i--)
    {
        if(s[i]==' ')
        break;
        else
        c++; 
    }
    }
    return c;
}
