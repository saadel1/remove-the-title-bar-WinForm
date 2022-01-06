# remove-the-title-bar-WinForm
 protected override void WndProc(ref Message m)
        {
            const int sizing = 0x0083;
            if (m.Msg == sizing && m.WParam.ToInt32()==1)
            {
                return;
            }
            base.WndProc(ref m);
        }
