

        private void btnStart_Click(object sender, EventArgs e)
        {
            //varibles
            int firstNumber;
            int secondNumber;

            //clear listbox
            this.lstAlphabet.Items.Clear();

            for (firstNumber = 65; firstNumber <= 90; firstNumber++)
            {
                for (secondNumber = 97; secondNumber <= 122; secondNumber++)
                {
                    this.lstAlphabet.Items.Add(Char.ConvertFromUtf32(firstNumber) + " --> " +                                                    Char.ConvertFromUtf32(secondNumber));
                }                   
            }
        }
    }
}
